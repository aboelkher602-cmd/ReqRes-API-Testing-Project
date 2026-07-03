# ReqRes API Testing & Automation

## 📌 Project Overview
This project focuses on executing comprehensive end-to-end RESTful API testing for the [ReqRes](https://reqres.in/) platform. The goal is to validate backend functionality, data integrity, and response consistency across various HTTP methods.

## 🛠️ Tools & Technologies Used
* **API Testing:** Postman
* **Test Documentation:** Google Sheets (Test Cases & Bug Reports)
* **Assertions & Scripting:** JavaScript (Postman Tests)
* **Methodologies:** Black Box Testing, API Testing, Boundary Value Analysis

## 🎯 Testing Scope
The testing process covered the core CRUD operations (Create, Read, Update, Delete) to ensure the API behaves as expected under different scenarios (Positive & Negative testing).
* **HTTP Methods Validated:** GET, POST, PUT, DELETE.
* **Response Validation:** HTTP Status Codes (200 OK, 201 Created, 204 No Content, 400 Bad Request, 404 Not Found).
* **Data Verification:** JSON payload structure, data types, and response headers.
* **Automation Assertions:** Developed automated test scripts within Postman using JavaScript (`pm.test` and `pm.expect`) to dynamically verify responses.

## 📁 Project Deliverables

### 1. Test Documentation
* **[Test Cases Sheet] https://docs.google.com/spreadsheets/d/1r5T3VTsdwm6NOCFV4-WxLEcSQl_kGabi/edit?usp=sharing&ouid=108652635270921183824&rtpof=true&sd=true:** Contains detailed test scenarios, expected results, and execution status.
* **[Bug Reports Sheet]:https://docs.google.com/spreadsheets/d/1jCMJA479HDhwILUwayoJ7CzHKBIqRNbD/edit?usp=sharing&ouid=108652635270921183824&rtpof=true&sd=true** Structured documentation of identified defects, including reproduction steps, severity, and screenshots/logs.

### 2. Postman Collection
The repository includes the exported Postman files to reproduce the automated tests:
* `ReqRes_Collection.json`: Contains all the API requests with their respective pre-request scripts and test assertions.
* `ReqRes_Environment.json`: (If applicable) Contains the environment variables used, such as `{{base_url}}`.

## 🚀 How to Run the Tests

### Using Postman UI
1. Clone this repository to your local machine.
2. Open Postman.
3. Click on **Import** and select the `ReqRes_Collection.json` (and the Environment file if provided).
4. Select the imported collection, click on **Run**, and observe the test execution results in the Collection Runner.

📬 Contact
**Mahmoud Abo Elkher Mohammad**
* **Role:** Junior Software Quality Engineer
* **LinkedIn:** (https://www.linkedin.com/in/mahmoud-abo-elkher)
* **Email:** (http:// aboelkher602@gmail.com)

installed, you can run the collection directly from your terminal:
```bash
newman run ReqRes_Collection.json
