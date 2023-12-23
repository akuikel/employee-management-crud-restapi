# employee-management-crud-restapi
Employee Management Application- Spring Boot

Overview
This Spring Boot application provides a RESTful API for managing employees. It allows you to perform CRUD (Create, Read, Update, Delete) operations on employee data.


Technologies Used:
Spring Boot: The core framework for building the application.
Spring Data JPA: Used for data access and persistence.
Spring Web: Provides the necessary components for building a web application, including RESTful services.
H2 Database: An in-memory database for development and testing purposes.
Maven: Dependency management and build tool.

Setup:

Clone the repository:
git clone https://github.com/akuikel/employee-management-crud-restapi.git

Create Mysql database:
Run the SQLScript to create the database named employees

Change mysql username and password as per your installation:
open src/main/resources/application.properties
change spring.datasource.username and spring.datasource.password as per your mysql installation

Navigate to the project directory:
cd employee-management

Build the project using Maven:
./mvnw clean install

Run the application:
./mvnw spring-boot:run


The application will be accessible at http://localhost:8080.

Endpoints:

GET /api/employees: Retrieve a list of all employees.
GET /api/employees/{employeeId}: Retrieve details for a specific employee.
POST /api/employees: Add a new employee.
PUT /api/employees: Update an existing employee.
DELETE /api/employees/{employeeId}: Delete an employee.

You can use them using a REST client such as Postman, Insomnia, etc.

GET /api/employees:
Getting all employees from the Database.
Body Return:
<img width="1440" alt="Screenshot 2023-12-23 at 4 57 17 PM" src="https://github.com/akuikel/employee-management-crud-restapi/assets/108853044/0a032815-9855-41ac-8673-ca565c84516d">

GET /api/employees/{employeeId}: 
Retrieve details for a specific employee.
Body Return:
<img width="1437" alt="Screenshot 2023-12-23 at 5 00 44 PM" src="https://github.com/akuikel/employee-management-crud-restapi/assets/108853044/f045b85e-0ee9-4363-87c0-188222721e86">

POST /api/employees: 
Add a new employee.
Body Return:
<img width="1437" alt="Screenshot 2023-12-23 at 5 01 48 PM" src="https://github.com/akuikel/employee-management-crud-restapi/assets/108853044/a61079b3-db0d-47d4-9eb9-c894c983f576">

DELETE /api/employees/{employeeId}: 
Delete an employee.
Body Return:
<img width="1437" alt="Screenshot 2023-12-23 at 5 04 35 PM" src="https://github.com/akuikel/employee-management-crud-restapi/assets/108853044/fa0dbb97-7a66-4570-b9c5-3e84e32d7210">


