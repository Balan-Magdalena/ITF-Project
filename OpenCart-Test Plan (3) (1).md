`   `**OpenCart**

- Test Plan -



`  `**Revision History**


|**Date**|**Description**|**Author**|**Comments**|
| :-: | :-: | :-: | :-: |
|*03.08.2024*|Test Plan for OpenCart version 3.0.2.0|*Balan Magdalena*|Test plan version 1.0 (initial version)|
|||||


**Table of Content:**

1. Introduction
   1. Project objective
   1. Functionalities in scope
   1. Functionalities and tests out of scope
1. Test process
   1. Test planning
   1. Test analysis
   1. Test design
   1. Test implementation
   1. Test execution
   1. Test closure
   1. Test monitoring and control
1. Test deliverables
   1. Test plan
   1. Test conditions
   1. Test cases
   1. Daily test summary reports
   1. Traceability matrix
   1. Test case results
   1. Bugs report
   1. Test completion report

 

1. **Introduction**

OpenCart is free open source e-commerce platform for online merchants that provides a professional and reliable foundation from which to build a successful online store. This foundation appeals to a wide variety of users; ranging from seasoned web developers looking for a user-friendly interface to use, to shop owners just launching their business online for the first time. With OpenCart's tools, you can help your online shop live up to its fullest potential.

1. `  `**Project Objective**

The objective of this application is to ensure that the OpenCart website meets all functional and performance requirements, providing an uninterrupted and secure end-user experience. Through a comprehensive set of functional testing process, we aim to identify and resolve any issues that could negatively impact the app. This test plan serves as a communication tool to inform the stakeholders about our ongoing efforts to improve the quality of the platform.

1. `  `**Functionalities in scope**

For this version of the application the functionalities in the scope of testing are:

-Admin Module: This is the main administration interface of an OpenCart site, which allows administrators to manage all aspects of the online store. In the admin module, administrators can manage products, categories, orders, customers, promotions, store settings, payment methods, shipping methods, and other restricted areas.

-Product Management Module:  The functionalities in scope are related to the management of products, including product creation, editing, deletion, and categorization, as well as the configuration of product attributes and inventory settings.

\- User and Account Management Module: The functionalities in scope are related to user registration, login, profile management, password recovery, and account settings. This module also includes the management of user roles and permissions.

\- Shopping Cart and Checkout Module:The functionalities in scope include adding items to the cart, updating quantities, removing items, applying discount codes, and completing the checkout process. This includes payment gateway integration and confirmation of orders.

\- Order Management Module: The functionalities in scope involve the management of customer orders, including order processing, status updates, cancellations, returns, and refunds. It also includes generating order-related reports for sales analysis.

-Throughout the testing process, we will perform functional testing and some types of non-functional testing (like usability testing), positive testing, and negative testing. Additionally, as needed, we will perform retesting and regression testing.

-Other types of testing, such as smoke testing and sanity testing, might be performed if necessary.

-The types and techniques of testing will be decided accordingly after requirement analysis.

-Testing will be performed at a system testing level.


**1.3 Functionalities and tests out of scope**

-Advanced Third-Party Integrations:Testing for third-party plugins and extensions beyond standard OpenCart features.



\- Mobile App Testing:Only web-based application testing is in scope; native and hybrid mobile app testing is excluded.

\- Performance and Security Testing: Excludes non-functional tests such as load, stress, and security assessments.

\- Automation Testing: All tests will be manual; automated testing is not included.

\- Multilingual/Multi-currency Testing: Testing for multiple languages and currencies is not covered.

\- Extended Content Management: Advanced content features, beyond standard product and category management, are out of scope.

\- API Testing: External API integrations and web services testing are excluded.

**2. Test process**

`    `**2.1  Test planning**

**Roles and responsibilities**

|Role 1 - Test Lead|`   `Responsible for overseeing the testing process, coordinating team activities, and ensuring deadlines are met|
| :- | :- |
|Role 2 - Product Management Tester|` `Will test: related functionalities including product creation, editing, deletion, and inventory management|
|Role 3 - User Account Teste|` `Will test: user registration, login, profile management, and password recovery features|
|Role 4 - User Account Teste|` `Will test: the shopping cart functionalities, including adding/removing products, updating quantities, and applying discount codes|
|Role 5 - Checkout Process Teste|` `Will test : the entire checkout process, including payment gateway integration and order confirmation|
|Role 6 - Order Management Teste|` `Will test: order processing, status updates, cancellations, and refunds|
|Role 7 - SEO and Analytics Tester|` `Will test: SEO features, including meta tags, SEO-friendly URLs, and Google Analytics integration|
|Role 8 - Security Tester|` `Will test:security features, including user data protection, SSL/TLS encryption, and CAPTCHA integration|
|Role 9 - Admin Panel Tester|` `Will test :admin panel functionalities including user role management, order management, and reporting features|
|Role 10 - Content Management Tester|` `Will test: the management of static pages, categories, and product pages|
|Role 11 - Marketing Features Tester|` `Will test :marketing functionalities like discount codes, coupons, and email campaigns|
|Role 12 - Performance and Load Tester|` `Will conduct load testing and evaluate the performance under different conditions (if included in the scope)|

**Entry criteria:**

- Testing environment is up and running (being an already live application, we will have the environment ready even before the implementation step)
- Business requirements are completed by the analysis team and are delivered to the appropriate testing team for evaluation
- Potential project risks are detected and mitigated
- Roles and responsibilities are allocated
- Test plan should be finalized before entering the next phase of testing
- Define the objectives of testing and the accepted level of quality

**Exit criteria:**

- 90%  or more of the tests are passed
- No critical issues have status open
- All detected errors have been reported and closed
- The budget was reached
- The deadline was reached
- The objectives were fulfilled
- The product usage documentation has been finalized with the scenarios evaluated during the testing phase
- Test completion report has been created and sent to the stakeholders
- Product risks have been identified and mitigated

**Project risks:**

- The team does not have the proper knowledge or experience in order to guarantee the desired level of quality for the application.
- Project timeline has not been communicated, therefore the team cannot start planning feature delivery and completion date, therefore QA cannot create a validation schedule based on a delivery schedule.
- Not enough time has been allocated in order to properly test and cover all the functionalities in scope.
- All that the data that is going to be used will have to be created explicitly in the scope of testing, which will cut off from the time allocated for testing, generating a risk of not reaching the deadline.

**Product risks:**

- All the data that is going to be used will be test data, which will not give us an experience of the application close enough to the ones that the user will experience.
- Taking into account that only two modules are in the scope of testing, the rest of the modules will still be at risk of not fulfilling the user needs.

**2.2 Test analysis** 

- In this phase we will analyze the business requirements that were provided and we will create test conditions based on the received requirements.

**2.3 Test design**

- In  this phase we will create the test cases based on the previously defined test conditions to ensure that we will be covering all the functionalities that are in scope of this project.
- The test data that will be needed will be identified in this phase based on the identified data necessities from the created test cases.

**2.4 Test implementation**

- We make sure that all the test data is available and reviewed (test data= email examples, password examples, different type of currency, different types of credit cards)
- We make sure that the setup environment is up and running
- We make sure that we have all the needed access and permissions to all the systems involved in the validation process
- We prioritize the tests based on risks (if known) and business priority

**2.5 Test execution**

- The tests will be executed on the top 4 used browsers: Chrome, Mozilla Firefox, Microsoft Edge, Apple Safari. If time will be available we will extend tests on Opera and Brave browsers
- We will create bug reports when the expected results that were defined in the test cases are different from the actual results
- We will perform retesting and regression testing to make sure that all the bugs have been fixed and no previously working functionality was not affected by the changes
- We will generate the test status reports once a week and send them to the management team in order to provide them with means to monitor the testing process and take measures in case new risks are identified.

**2.6 Test closure**

- We will evaluate the exit criteria and we will make sure that it was fulfilled in order to green light the launching of the new product version into the production environment
- We will generate the test completion report and send it to stakeholders in order to inform them about the testing process results and enhance them with the ability to make informed decisions with regards to the product launching
- All the product risks will be detected and mitigated (a solution was found in order to reduce the probability of them to arise) or a contingency plan has been set in place 
- All the performed test cases will be executed in the test management tool and all the remaining bugs that have been retested and fixed have been closed
- Regression testing will be performed and no other issues have been detected
- Learned lessons will be gathered and collected into a common improvement plan in order to enhance the improvement of the next testing processes.

**2.7 Test monitoring and control** 

- We will evaluate the test status reports and monitor them all throughout the testing process in order to ensure a smooth testing and team collaboration and in order to make sure that new risks are identified in time and managed accordingly
- In case new risks will appear they will be mitigated or a contingency plan will be set in place to make sure that the negative effects will not stop us from fulfilling the testing objectives that were defined in the planning phase.

  **3.Test deliverables**

The following test deliverables will be provided by the end of the testing process and sent to the stakeholders in order to create the basis of informed decision:

- Test plan 
- Test conditions 
- Test cases
- Daily test summary report
- Traceability matrix
- Test case results
- Bugs report
- Test completion report.

**4. Schedule**

- The testing process will take place over a period of 2 months and will involve all the activities defined in the previous section.
- All the resources will be adapted accordingly in case new testing resources are detected as necessary.






