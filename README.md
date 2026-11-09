Student Registration and Management System
------------------------------------------

A web application for registering students and viewing them, built with Spring MVC, Thymeleaf, Java and PostgreSQL. 
I used plain JDBC with hand-written SQ

Features
------------
Register a student through an HTML form with validation
Store students in PostgreSQL (first and last name saved as a single full_name)
List all registered students in a table
Search a student by ID (bonus), reusing the same students.html page
Friendly messages for validation errors, duplicate emails, and students that do not exist 


Technologies Used
------------------
Java 17
Spring Boot 3.3 (Spring MVC, Bean Validation)
Thymeleaf (server-side HTML templates)
PostgreSQL with JDBC (Connection, PreparedStatement, ResultSet)
HikariCP (connection pool behind the DataSource)
Maven

Project Structure
-----------------

The code is organized into separate packages.
The model package holds the Student class, the controller package holds StudentController
, the service package holds StudentService, the repository package holds StudentRepository with all the JDBC code, 
and the config package holds DatabaseConfig, which creates the DataSource. An exception package holds the error class. 
The resources folder holds the application properties file, the two Thymeleaf templates, register.html and students.html,
and the CSS file.

 The Screens registered
-----------------------
<img width="620" height="444" alt="registered student" src="https://github.com/user-attachments/assets/80f66acb-4662-4e62-98a0-a4b9e3981bc5" />

The full registered student in front side where we have first and last name as separate fields
----------------------------------------------------------------------------------------------
<img width="788" height="371" alt="allStudent" src="https://github.com/user-attachments/assets/68ccf307-b54f-4c03-bce7-1c2edb82dbb9" />

The full registered student in the database view where we retrieve all as it saved the Full names
--------------------------------------------------------------------------------------------------
<img width="429" height="194" alt="databseView" src="https://github.com/user-attachments/assets/b7b6bc2f-248d-4c21-ab5d-aff2319d7fc6" />

The student information by Id(5)
----------------------------------
<img width="805" height="329" alt="SaveById" src="https://github.com/user-attachments/assets/f35bfa10-5fe3-4a09-ab10-725a6eebbc53" />





