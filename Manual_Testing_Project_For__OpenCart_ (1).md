<h1>Testing Project for **OpenCart*</h1>

The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in practice, using a live application

Application under test: **OpenCart**

Tools used: Jira, Zephyr Squad.

<h2>Functional specifications:</h2>

The below stories : "**Login admin module, Products filter, Shipping and Payment method ,Product comparison ,Delete user account"**, was created in Jira and describes the functional specifications of the "**OpenCart_Admin_Module and Opencart_Demo _Store _Front _Module**", for which the final project is performed upon.

[BM-10.pdf](https://github.com/user-attachments/files/17081012/BM-10.pdf)

[BM-39.pdf](https://github.com/user-attachments/files/17081011/BM-39.pdf)

[BM-32.pdf](https://github.com/user-attachments/files/17081010/BM-32.pdf)

[BM-15.pdf](https://github.com/user-attachments/files/17081009/BM-15.pdf)

[BM-29.pdf](https://github.com/user-attachments/files/17081008/BM-29.pdf)


Here you can find the release that was created for this project:

![image](https://github.com/user-attachments/assets/3473274b-1e80-4663-8d24-2b97d23ca25a)

<h2>Testing process</h2>

The test process was performed based on the standard test process as described below.

<h3>1.1 Test planning</h3>

The Test Plan is designed to describe all details of testing for all the modules from the JPetStore Demo application.

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed, the personnel responsible for testing, the resources and schedule required to complete testing, and the risks associated with the plan. The test plan that was created for this project can be found here **[OpenCart-Test Plan.pdf](https://github.com/user-attachments/files/17081034/OpenCart-Test.Plan.pdf)**


<h4>1.1.1. Roles asigned to the project and persons allocated</h4>

<ul>
  <li>Project manager - John Carter </li> 
  <li>Product owner - Emily Thompson </li>
  <li>Software developer - Michael Richardson </li>
  <li>QA Engineer - Balan Magdalena</li>
</ul>

<h4> 1.1.2 Entry criteria defined </h4>

- Testing environment is up and running (being an already live application, we will have
the environment ready even before the implementation step)
- Business requirements are completed by the analysis team and are delivered to the
appropriate testing team for evaluation
- Potential project risks are detected and mitigated
- Roles and responsibilities are allocated
- Test plan should be finalized before entering the next phase of testing
- Define the objectives of testing and the accepted level of quality

<h4> 1.1.3 Exit criteria defined </h4>

- 90% or more of the tests are passed
- No critical issues have status open
- All detected errors have been reported and closed
- The budget was reached
- The deadline was reached
- The objectives were fulfilled
- The product usage documentation has been finalized with the scenarios evaluated
during the testing phase
- Test completion report has been created and sent to the stakeholders
- Product risks have been identified and mitigated

<h4> 1.1.4 Test scope</h4>

<h5> Tests in scope: </h5>

-Admin Module: This is the main administration interface of an OpenCart site, which allows
administrators to manage all aspects of the online store. In the admin module,
administrators can manage products, categories, orders, customers, promotions, store
settings, payment methods, shipping methods, and other restricted areas.

-Product Management Module: The functionalities in scope are related to the management
of products, including product creation, editing, deletion, and categorization, as well as the
configuration of product attributes and inventory settings.
- User and Account Management Module: The functionalities in scope are related to user
registration, login, profile management, password recovery, and account settings. This
module also includes the management of user roles and permissions.
- Shopping Cart and Checkout Module:The functionalities in scope include adding items to
the cart, updating quantities, removing items, applying discount codes, and completing the
checkout process. This includes payment gateway integration and confirmation of orders.
- Order Management Module: The functionalities in scope involve the management of
customer orders, including order processing, status updates, cancellations, returns, and
refunds. It also includes generating order-related reports for sales analysis.
-Throughout the testing process, we will perform functional testing and some types of non-functional
testing (like usability testing), positive testing, and negative testing. Additionally, as needed, we will
perform retesting and regression testing.
-Other types of testing, such as smoke testing and sanity testing, might be performed if necessary.
-The types and techniques of testing will be decided accordingly after requirement analysis.
-Testing will be performed at a system testing level.

<h5>Tests not in scope: </h5>

-Advanced Third-Party Integrations:Testing for third-party plugins and extensions beyond standard
OpenCart features.
- Mobile App Testing:Only web-based application testing is in scope; native and hybrid mobile app
testing is excluded.
- Performance and Security Testing: Excludes non-functional tests such as load, stress, and security
assessments.
- Automation Testing: All tests will be manual; automated testing is not included.
- Multilingual/Multi-currency Testing: Testing for multiple languages and currencies is not covered.
- Extended Content Management: Advanced content features, beyond standard product and
category management, are out of scope.
- API Testing: External API integrations and web services testing are excluded.

<h4>1.1.5 Risks detected</h4>

<h5>Project risks:</h5>

- The team does not have the proper knowledge or experience in order to guarantee
the desired level of quality for the application.
- Project timeline has not been communicated, therefore the team cannot start
planning feature delivery and completion date, therefore QA cannot create a
validation schedule based on a delivery schedule.
- Not enough time has been allocated in order to properly test and cover all the
functionalities in scope.
- All that the data that is going to be used will have to be created explicitly in the scope
of testing, which will cut off from the time allocated for testing, generating a risk of
not reaching the deadline.

<h5> Product risks: </h5>

- All the data that is going to be used will be test data, which will not give us an
experience of the application close enough to the ones that the user will experience.
- Taking into account that only two modules are in the scope of testing, the rest of the
modules will still be at risk of not fulfilling the user needs.

<h4>1.1.6 Evaluating entry criteria</h4>

The entry criteria defined in the Test Planning phase have been achieved and the test process can continue.

<h3>1.2 Test Monitoring and Control<h3>

- We will evaluate the test status reports and monitor them all throughout the testing
process in order to ensure a smooth testing and team collaboration and in order to
make sure that new risks are identified in time and managed accordingly
- In case new risks will appear they will be mitigated or a contingency plan will be set
in place to make sure that the negative effects will not stop us from fulfilling the
testing objectives that were defined in the planning phase.
![image](https://github.com/user-attachments/assets/f3476a67-a033-4156-bbb2-1aed4d53cbb1)



<h3> 1.3 Test Analysis </h3>
The testing process will be executed based on the application requirements.</b>. <br><br>

The following test conditions were found: <br>

![image](https://github.com/user-attachments/assets/d87545cf-a8bf-42c4-b154-f5ea23591002)




<h3>1.4 Test Design</h3>

Functional test cases were created in Zephyr Squad based on the analysis of the specifications. The test cases can be accessed here 

[Jira.pdf](https://github.com/user-attachments/files/17081287/Jira.pdf)


<h3>1.5 Test Implementation</h3>

The following elements are needed to be ready before the test execution phase begins:

- We make sure that all the test data is available and reviewed (test data= email
examples, password examples, different type of currency, different types of credit
cards)
- We make sure that the setup environment is up and running
- We make sure that we have all the needed access and permissions to all the systems
involved in the validation process
- We prioritize the tests based on risks (if known) and business priority

<h3>1.6. Test Execution </h3>

Test cases are executed on the created test Cycle summary: **Admin login, Login user, Register user, Wish list, Add to cart, Delete gift certificate, Gift certificate, Wish list, Add Product to Shopping Cart, Complete Purchase**

Bugs have been created based on the failed tests. The complete bug reports can be found here: [PDF (Jira)2.pdf](https://github.com/user-attachments/files/17081441/PDF.Jira.2.pdf)


The following is a summary of the bugs that have been found:

-Login not possible after the account has been registered - **Highest**

-Admin unable to edit account detail - **High**		

-Add, edit and delete are not allowed to admin- **High**

-Account information belong to another user - **High**

-Shipping and payment methods from the checkout cant be chosen - **High**

-The gift certificates added to the shopping cart cant be deleted - **Medium**		
	
-The appearance of the page on the phone does not show any icon of the functions - **Medium**		
	
-No functions icon are displayed when opening the store front page for the first time - **Medium**		
	
-Payment method cant be chose when ordering a Gift Certificate - **Medium**		
	
-Out-of-stock products are not marked properly - **Medium**	

-Unnecessary fields for ordering the product Apple Cinema 30 - **Medium**	
			
-Wrong images for the product Apple Cinema 30 - **Medium**		
	
-The banner from the home page redirects to a different product than expected - **Medium**				
	
-Visual bug for description field - **Medium**


Full regression testing is needed on the impacted areas after the bugs are fixed and retesting will be done for every functionality that was previously failed.

<h3> 1.7 Test Completion</h3>
As the Exit criteria were met and satisfied as mentioned in the appropriate section, this feature is suggested to ‘Go Live’ by the Testing team

The traceability matrix was generated and can be found here: [Forward Traceability_21_9_2024.xlsx](https://github.com/user-attachments/files/17081467/Forward.Traceability_21_9_2024.xlsx)


Test execution chart was generated and can be found below. 

[Test.execution.chart.pdf](https://github.com/user-attachments/files/17209666/Test.execution.chart.pdf)



The final report shows that a number 4 tests have failed of a total of 10.

A number of 14 total bugs were found, from which the priority is: 5 are high and 9 are medium.

Following the testing of the OpenCart Demo platform, a total of 10 tests were created and executed. Out of these, 4 tests failed, leading to the discovery of 14 bugs.

Requirements Coverage: Approximately 85% of the requirements within the scope of testing were covered, and all major modules such as product management, user account management, and the checkout process were successfully tested. However, certain functionalities, such as third-party payment integration, were not fully tested due to time constraints.

Bug Impact: Of the 14 bugs identified, 5 are considered critical and could negatively impact the user experience in production. It is recommended to release the product only after fixing these critical issues, especially those related to order processing and payment functionalities. The remaining medium and low-severity bugs can be fixed in future versions without significantly affecting the initial release.

Identified Risks: There are risks related to the application’s performance under heavy load, as load testing was not conducted. Additionally, there is a risk that certain modules, such as promotion management, which were not tested in-depth, might contain defects that could impact long-term usability.

Recommendations:

-It is recommended to fix all critical bugs before release.
Regression testing is suggested after each modification to ensure that other functionalities are not affected.
-In future projects, allocating additional time for testing would help cover all functionalities and reduce risks.

Lessons Learned:

-Clear prioritization of essential functionalities was beneficial during this testing phase.
-However, it was observed that planning automated testing for recurring functionalities would save time and reduce human error in future projects.
