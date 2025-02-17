## STE Assessment- Bug Challenge
### Bug-Finding Challenge
At Paylocity, the highest priority of the software tester is to find bugs before the end
user does. This challenge is designed to have you demonstrate your bug-finding
ability in both the API the UI of an application.

### Test Plan: Paylocity Benefits Dashboard

**1. Introduction**

This document outlines the test plan for the Paylocity Benefits Dashboard application, focusing on both UI and API testing. The goal is to identify as many defects as possible, covering various functionalities and scenarios.  This test plan will be used for both the Bug Finding Challenge and will inform the Automation Challenge.

**2. Scope**

This test plan covers the following areas:

* **UI Testing:**  Functional testing of the Benefits Dashboard UI, including adding, editing, and deleting employees and dependents, and verifying benefit cost calculations.
* **API Testing:** Functional testing of the API endpoints related to employee and dependent management, ensuring data integrity and correct responses.

This test plan does *not* cover:

* Performance testing
* Security testing
* Usability testing (beyond basic navigation and workflow)
* Compatibility testing (beyond major browsers)

**3. Test Strategy**

The testing strategy will involve a combination of:

* **Functional Testing:**  Verifying that all features work as expected according to the user story and acceptance criteria.
* **Boundary Value Analysis:** Testing with input values at the limits of acceptable ranges.
* **Equivalence Partitioning:** Dividing input data into ranges that are expected to be treated similarly.
* **Error Guessing:**  Using experience and intuition to anticipate potential error conditions.
* **API Contract Testing:** Validating API responses against the provided documentation (Postman/Swagger).

**4. Test Environment**

* **UI Testing:**  Modern web browsers (e.g., Chrome, Firefox, Edge).  Specific versions will be documented with bug reports.
* **API Testing:** Postman or a similar API testing tool.
* **API Documentation:**  [https://documenter.getpostman.com/view/2314100/SWTEbbi6](https://documenter.getpostman.com/view/2314100/SWTEbbi6) & [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/swagger/v1/swagger.json](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/swagger/v1/swagger.json)
* **Application URL:** [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login)
* **Credentials:** Provided separately.

**5. Test Data**

Test data will include:

* **Valid Employee Data:**  Realistic employee names, ages, etc.
* **Invalid Employee Data:**  Data that violates constraints (e.g., negative ages, special characters in names).
* **Boundary Values:**  Employee data at the limits of acceptable ranges (e.g., very high/low ages).
* **Edge Cases:**  Specific data combinations that might cause issues.
* **Dependent Data:** Valid and invalid dependent information.

**6. Test Cases**

Test cases will be created based on the user story and acceptance criteria, including positive and negative tests.  Example test cases:

**UI Test Cases:**

* **Add Employee (Positive):**  Verify adding a new employee with valid data.
* **Add Employee (Negative - Invalid Age):** Verify error message when adding an employee with an invalid age.
* **Edit Employee:** Verify editing existing employee data.
* **Delete Employee:** Verify deleting an employee.
* **Benefit Calculation:** Verify correct benefit cost calculation for employees and dependents.

**API Test Cases:**

* **GET Employees:** Verify retrieving a list of employees.
* **POST Employee:** Verify creating a new employee via the API.
* **PUT Employee:** Verify updating an existing employee via the API.
* **DELETE Employee:** Verify deleting an employee via the API.
* **GET Employee by ID:** Verify retrieving a single employee by their ID.

**7. Bug Reporting**

All identified bugs will be reported with the following information:

* **Title:**  A concise description of the bug.
* **Description:**  Detailed explanation of the bug.
* **Steps to Reproduce:**  Clear steps to reproduce the bug.
* **Expected Result:**  What the application should do.
* **Actual Result:**  What the application actually does.
* **Severity:**  Impact of the bug (e.g., critical, major, minor).
* **Environment:**  Browser, OS, API tool used.
* **Screenshots/Screen Recordings:**  Visual evidence of the bug.
* **API Request/Response (if applicable):**  Details of the API interaction.

**8. Deliverables**

* Bug reports (UI and API)
* (For the Automation Challenge) API and UI test automation projects with execution instructions.

**9. Timeline**

The testing phase will be completed within the allocated 72-hour timeframe.

**10. Exit Criteria**

Testing will be considered complete when all planned test cases have been executed and all identified bugs have been reported. The focus will be on thorough coverage of the core functionality and API.