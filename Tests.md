* Which tests are there?

[Source](https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing)

There is a clear distinction between manual and automated tests. 
Manual tests are done in person and are therefore more time intensive.
Automated tests are therefore more cost effective and are used a lot in combiniton with complexer codebases.

The different types of tests include: Unit Testing, Integration Testing, Functional Testing, End-to-end Testing, Acceptance Testing, Performance Testing, Regression Testing, Load Testing, Security testing, Usability testing, Compatibility testing and Smoke Testing.

**Unit Testing:**
Unit tests are very low level and close to the source of an application. 
They consist in testing individual methods and functions of the classes, components, or modules used by your software.

**Integration Testing:**
Integration tests verify that different modules or services used by your application work well together.  
These types of tests are more expensive to run as they require multiple parts of the application to be up and running.

**Functional Testing:**
Functional tests focus on the business requirements of an application. 
They only verify the output of an action and do not check the intermediate states of the system when performing that action.

**End-to-end Testing:**
End-to-end testing replicates a user behavior with the software in a complete application environment. 
It verifies that various user flows work as expected and can be as simple as loading a web page or logging in or much more complex scenarios verifying email notifications, online payments, etc...

**Acceptance Testing:**
Acceptance tests are formal tests that verify if a system satisfies business requirements. 
They require the entire application to be running while testing and focus on replicating user behaviors.

**Performance Testing:**
Performance tests evaluate how a system performs under a particular workload. 
These tests help to measure the reliability, speed, scalability, and responsiveness of an application.

**Regression Testing:**
Regression testing is a software testing practice that involves re-executing a set of software tests to ensure that previously developed and tested software still performs as expected after a change.
[Source](https://katalon.com/resources-center/blog/regression-testing)

**Load Testing:**
Load testing is a type of performance testing that is used to simulate a real-world load on any software, application, or website to see how it performs under stress.
The goal of load testing is to identify bottlenecks and determine the maximum number of users or transactions the system can handle.
[Source](https://www.geeksforgeeks.org/software-testing-load-testing/)

**Security testing:**
Security testing is a type of software testing that aims to identify potential security risks and vulnerabilities in an application, system, or network.
The primary goal of security testing is to uncover any weaknesses that could be exploited by attackers to gain access to sensitive data or interrupt system operations.
[Source](https://www.crowdstrike.com/cybersecurity-101/security-testing/)

**Usability testing:**
Usability testing is a type of testing that focuses on evaluating how easy and user-friendly a software application or website is.
The goal of usability testing is to evaluate the design intuitiveness of the product and identify points of friction or confusion.
[Source](https://www.guru99.com/usability-testing-tutorial.html)

**Compatibility testing:**
Compatibility testing is a type of non-functional testing that is performed to verify whether an application or software can run on different devices, browsers, operating systems, hardware, and networks.
Compatibility testing is crucial to ensure that the software performs well across different types of environments, devices, and networks
[Source](https://artoftesting.com/compatibility-testing)

**Smoke Testing:**
Smoke tests are basic tests that check the basic functionality of an application. 
They are meant to be quick to execute, and their goal is to give you the assurance that the major features of your system are working as expected.

* Which tests are useful for my application?

I was already planning on doing a manual test for my application, because I know someone from my target demographic and this test ensures that my user stories are indeed done.

* How would I carry out these tests?

The manual test will be carried out by running my application, letting the user read the user story and have them try to recreate the user story with my application. I will then write down any remarks the user gives and put this towards completing my user stories.

* Results

The manual test was performed on 6-6-2023.
The user was able to complete the user stories, but explained that there was some confusion about the information on my website.
This is because there is no styling in place.
Therefore the user was able to get to the information page, but could not make out what the information was. 
Refining the UI would solve this problem with an usability test to make sure my UI is good.
