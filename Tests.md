* Which tests are there?

[Source](https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing)

There is a clear distinction between manual and automated tests. 
Manual tests are done in person and are therefore more time intensive.
Automated tests are therefore more cost effective and are used a lot in combiniton with complexer codebases.

The different types of tests include: Unit Testing, Integration Testing, Functional Testing, End-to-end Testing, Acceptance Testing, Performance Testing, Regression Testing, Load Testing, Security testing, Usability testing, Compatibility testing and Smoke Testing.

* Which tests are useful for my application?

I was already planning on doing a manual test for my application, because I know someone from my target demographic and this test ensures that my user stories are indeed done.

Other test that I would like to carry out include:

**Usability testing:**
Usability testing is a type of testing that focuses on evaluating how easy and user-friendly a software application or website is.
The goal of usability testing is to evaluate the design intuitiveness of the product and identify points of friction or confusion.
[Source](https://www.guru99.com/usability-testing-tutorial.html)

**Unit Testing:**
Unit tests are very low level and close to the source of an application. 
They consist in testing individual methods and functions of the classes, components, or modules used by your software.

**Integration Testing:**
Integration tests verify that different modules or services used by your application work well together.  
These types of tests are more expensive to run as they require multiple parts of the application to be up and running.

* How would I carry out these tests?

The manual test will be carried out by running my application, letting the user read the user story and have them try to recreate the user story with my application. 
I will then write down any remarks the user gives and put this towards completing my user stories.
This will also be the usability test.

I want to do Unit testing, because this tests the individual units in my application. 
I want to do Integration testing, because this is a step further from Unit testing and tests if the interfaces & flow of data/information between the modules is correct. 
Unit testing is done before Integration testing, because you first need to know there are no error in de modules themselves, before testing if the modules communicate properly.

I would write the Unit tests with XUnit, because XUnit is (in my humble opinion) better than MSTest and I have worked with XUnit before.

I would write the Unit tests with ...

* Testplan

Testplan for Unit tests:

|Test case ID|Test case objective|Test case description|Expected result|
|------------|-------------------|---------------------|---------------| 
|1| Check if the GetFish function returns the expexted result| Call the GetFish function and compare this to the mocked data| The GetFish function returns the same list as the mocked data|
|2| Check if the PostFish function add a fish to the database| Call the PostFish function and look in the mocked data to see if it added correctly| The PostFish function adds a fish correctly to the database|
|3| Check if the PutFish function updates a fish in the database| Call the PutFish function and look in the mocked data to see if the data changed| The PutFish function updates the data of a fish correctly|
|4| Check if the DeleteFish function deletes a fish from the database| Call the DeleteFish function and compare the mocked data to the original list| The DeleteFish function removes a fish from the database correctly|

Testplan for Integration tests:

|Test case ID|Test case objective|Test case description|Expected result|
|------------|-------------------|---------------------|---------------| 
|1| Check if the GetFish endpoint returns the expexted result| Call the GetFish endpoint and compare this to the mocked data| The GetFish endpoint returns the same list as the mocked data|
|2| Check if the PostFish endpoint add a fish to the database| Call the PostFish endpoint and look in the mocked data to see if it added correctly| The PostFish endpoint adds a fish correctly to the database|
|3| Check if the PutFish endpoint updates a fish in the database| Call the PutFish endpoint and look in the mocked data to see if the data changed| The PutFish endpoint updates the data of a fish correctly|
|4| Check if the DeleteFish endpoint deletes a fish from the database| Call the DeleteFish endpoint and compare the mocked data to the original list| The DeleteFish endpoint removes a fish from the database correctly|

As seen above, are the test objectives for the Unit and Integration tests almost identical.
This is because my application has no real logic to test. 
Therefor is it not really useful to carry out Unit tests. 
Integration tests are still relevant though, because I the communication between front- and back-end goes via an API.

* Results

The manual test was performed on 6-6-2023.
The user was able to complete the user stories, but explained that there was some confusion about the information on my website.
This is because there is no styling in place.
Therefore the user was able to get to the information page, but could not make out what the information was. 
Refining the UI would solve this problem with an usability test to make sure my UI is good.

To be more specific about the feedback I got back from the user;
There was confusion about the information on the website, because it doesn't have a clear layout. 
The texts are not neatly organised and it would improve immensly if I added indicators for the information. 

For example: I could put a header above certain information to clarify what type of information it is.

The search bar is also a problem, because it is far to long.
This makes it so the bar doesn't resemble a search bar and thus gets overlooked. 
Adding a magnifying glass icon in (or next to) the search bar could be used to partially solve this problem.
