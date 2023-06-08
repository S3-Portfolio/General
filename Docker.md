How would someone get my application from / through Docker?

"490511/divespot_fe:latest"

"490511/divespot:latest"

(Github kijken voor voor inspiratie over hoe docker)

[Share docker application](https://docs.docker.com/get-started/04_sharing_app/)

------------------------------------------------------------------------------------------------------------------------------------------------------------------

Docker desktop:

![image](https://github.com/S3-Portfolio/General/assets/93527848/d67de17b-e907-44d1-8174-e25656503595)

Frontend Docker file:

![image](https://github.com/S3-Portfolio/General/assets/93527848/cf0de743-1679-460f-8e62-b07fc41c38c7)

Frontend Workflow file:

```
name: Main

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v3
   
  deployment:
    name: deployment
    runs-on: ubuntu-latest
    needs: build
    steps:
      - name: Checkout repository
        uses: actions/checkout@v2
      - name: Set up Docker Buildx
        uses: docker/setup-buildx-action@v1
      - name: Login to DockerHub
        uses: docker/login-action@v1
        with:
          username: ${{ secrets.DOCKER_HUB_USERNAME }}
          password: ${{ secrets.DOCKER_HUB_PASSWORD }}
      - name: Build and push
        uses: docker/build-push-action@v2
        with:
          context: ./divespot/
          file: ./divespot/Dockerfile
          push: ${{ github.event_name != 'pull_request' }}
          tags: ${{ secrets.DOCKER_HUB_USERNAME }}/divespot_fe:latest 
``` 

Backend Docker file:

![image](https://github.com/S3-Portfolio/General/assets/93527848/6e393bab-9caa-4c4d-b59e-eaef3b060388)

Backend Workflow file:

```
  name: .NET Core Desktop
  on:
   push:
      branches: [ "master" ]
   pull_request:
      branches: [ "master" ]
  jobs:
    build:
      strategy:
        matrix:
          configuration: [Debug, Release]
    runs-on: windows-latest  
    env:
      Solution_Name: DiveSpot                  
      Test_Project_Path: DiveSpot.Tests         
      Wap_Project_Directory: DiveSpot  
      Wap_Project_Path: DiveSpot             

    steps:
    - name: Checkout
      uses: actions/checkout@v3
      with:
        fetch-depth: 0

    # Install the .NET Core workload
    - name: Install .NET Core
      uses: actions/setup-dotnet@v3
      with:
        dotnet-version: 6.0.x

    # Add  MSBuild to the PATH: https://github.com/microsoft/setup-msbuild
    - name: Setup MSBuild.exe
      uses: microsoft/setup-msbuild@v1.0.2

    # Execute all tests in the solution
    - name: Execute tests
      run: dotnet test

    # Restore the application to populate the obj folder with RuntimeIdentifiers
    - name: Restore the application
      run: msbuild $env:Solution_Name /t:Restore /p:Configuration=$env:Configuration
      env:
        Configuration: ${{ matrix.configuration }}

    # Decode the base 64 encoded pfx and save the Signing_Certificate
    - name: Decode the pfx
      run: |
        $pfx_cert_byte = [System.Convert]::FromBase64String("${{ secrets.Base64_Encoded_Pfx }}")
        $certificatePath = Join-Path -Path $env:Wap_Project_Directory -ChildPath GitHubActionsWorkflow.pfx
        [IO.File]::WriteAllBytes("$certificatePath", $pfx_cert_byte)
    # Create the app package by building and packaging the Windows Application Packaging project
    - name: Create the app package
      run: msbuild $env:Wap_Project_Path /p:Configuration=$env:Configuration /p:UapAppxPackageBuildMode=$env:Appx_Package_Build_Mode /p:AppxBundle=$env:Appx_Bundle /p:PackageCertificateKeyFile=GitHubActionsWorkflow.pfx /p:PackageCertificatePassword=${{ secrets.Pfx_Key }}
      env:
        Appx_Bundle: Always
        Appx_Bundle_Platforms: x86|x64
        Appx_Package_Build_Mode: StoreUpload
        Configuration: ${{ matrix.configuration }}

    # Remove the pfx
    - name: Remove the pfx
      run: Remove-Item -path $env:Wap_Project_Directory\GitHubActionsWorkflow.pfx

    # Upload the MSIX package: https://github.com/marketplace/actions/upload-a-build-artifact
    - name: Upload build artifacts
      uses: actions/upload-artifact@v3
      with:
        name: MSIX Package
        path: ${{ env.Wap_Project_Directory }}\AppPackages
```
