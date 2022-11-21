## ECE444 Lab 6: TDD

_scroll further for the written section of the project_

Ani Srikanth's submission for ECE444 Lab 6 for the Fall 2022 semester.

This lab is a replay of the [flaskr-tdd project](https://github.com/mjhea0/flaskr-tdd#first-test)

### First Test

<img width="840" alt="image" src="https://user-images.githubusercontent.com/14436239/201186706-2eb274b9-d954-47d3-9ed1-bd5e0388a888.png">

### Database Setup

<img width="855" alt="image" src="https://user-images.githubusercontent.com/14436239/201194170-a3db980d-c18f-47af-86f0-a369691e1d95.png">

### Templates and Views

<img width="845" alt="image" src="https://user-images.githubusercontent.com/14436239/201197925-6b517e62-25f1-405d-8948-38388501e29a.png">

### Add Some Style

![image](https://user-images.githubusercontent.com/14436239/201199705-5f5331be-1697-48cc-9cbd-cfb72ef24c31.png)

### Javascript

<img width="856" alt="image" src="https://user-images.githubusercontent.com/14436239/201203731-8f8e06a5-65da-4d77-aefd-831fc77b2759.png">

Adding 2 posts

<img width="599" alt="image" src="https://user-images.githubusercontent.com/14436239/201202259-68cdc45e-c9cc-4571-aa77-08e0ed8accd2.png">

<img width="741" alt="image" src="https://user-images.githubusercontent.com/14436239/201202797-6f622053-f669-46db-96d5-270fcebb7252.png">

After clicking 'Post 1'

<img width="602" alt="image" src="https://user-images.githubusercontent.com/14436239/201203305-98d76ce5-cc02-45db-bde7-f09ef41c0321.png">
<img width="405" alt="image" src="https://user-images.githubusercontent.com/14436239/201203382-f0c80b7e-bd1d-4b64-9e81-f1dc5be2b293.png">

### Deployment

![image](https://user-images.githubusercontent.com/14436239/202942686-4866723e-f1b1-46ba-aa55-5f6dc41671fd.png)

### Bootstrap

![image](https://user-images.githubusercontent.com/14436239/202961865-3a56a097-455e-47e2-8b35-20e4a0fb3a32.png)

### SQLAlchemy

![image](https://user-images.githubusercontent.com/14436239/202963412-2c6d3a13-9844-40f5-8026-e7b8e3e83aae.png)

### Search Page

![image](https://user-images.githubusercontent.com/14436239/202964720-31531cef-c6ce-4374-adc0-3a32ea1139f9.png)

### Login Required

![image](https://user-images.githubusercontent.com/14436239/202965098-d726b4b6-f49a-4378-b194-557b23150ee0.png)

### Postgres Heroku

![image](https://user-images.githubusercontent.com/14436239/202966178-f8ac89f5-31b7-43f0-b2d3-577196298a85.png)

### Linting and Code Formatting

![image](https://user-images.githubusercontent.com/14436239/202967981-4ab5c3bb-d1b4-4f85-a33e-dbe703d7ff0a.png)

## Links to tests cases I've added to Education Pathways

As this assignment was done after the code was submitted, you can verify these tests were written by me by looking at the Git blame of the code.

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/d71c91e015eb95406b15a827bba90e3813e926a1/Education_Pathways/tests/test_mc_api.py#L35

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/d71c91e015eb95406b15a827bba90e3813e926a1/Education_Pathways/tests/test_mc_api.py#L44

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/d71c91e015eb95406b15a827bba90e3813e926a1/Education_Pathways/tests/test_mc_api.py#L73

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/d71c91e015eb95406b15a827bba90e3813e926a1/Education_Pathways/tests/test_mc_api.py#L102

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/294b87e723d00b79016e5afe641bd9b25ef6357e/Education_Pathways/tests/test_degree.py#L32

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/294b87e723d00b79016e5afe641bd9b25ef6357e/Education_Pathways/tests/test_degree.py#L38

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/294b87e723d00b79016e5afe641bd9b25ef6357e/Education_Pathways/tests/test_degree.py#L44

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-23-runtimeterror/blob/294b87e723d00b79016e5afe641bd9b25ef6357e/Education_Pathways/tests/test_degree.py#L75

## What are the pros and cons of TDD?

While there are several pros for Test Driven Development (TDD), I will focus on two in particular. The first pro comes from the idea that defining the expected behaviour of code in its entirety, from input to output, can ease the development of the functions that execute such behaviour. When you write tests for the functions first, you assert certain behaviour of the function. Taking the time to determine, formulate, and write these tests with your team can ensure everyone has a concrete idea about the expectations of a module before it begins development. Further, it can allow for parallel processes to occur since, with the tests being written first, consumers of your module can safely assume the inputs of their modules. In essence, this is the idea of test-driven development, creating tests **before** writing the functions, steering (or driving) the method by which you write the code.

The second pro of TDD allows for regression testing. Regression testing is defined as "re-running functional and non-functional tests to ensure that previously developed and tested software still performs as expected after a change."[Wikipedia] When every component of the code is properly covered by tests. Any change in code can ensure previously functioning components, unrelated to the code change, remain working. In the event a test related to new changes fails due to the change, it can be properly analyzed to verify the new behaviour is as required.

One significant problem with applying TDD arises when you compare the quality of the tests relative to the quantity of the tests. Tests are often written with the metric of code coverage in mind, but this doesn't necessarily test the rigour of the code and its ability to withstand issues. It's important that while applying TDD in your code base, you plan and write tests that will do a sufficient job of testing the resiliency of the code.

Further, TDD genuinely requires a lot of work. Developers need the necessary knowledge and determination to write these tests consistently. This could require additional ramp-up time for developers whom TDD is new to. TDD can only be relied on if every developer does a good job of applying it to all aspects of the system to develop and maintain the tests!
