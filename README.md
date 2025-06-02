# EmployeeManagementSystem
# Employee Management System

The **Employee Management System** is a Java-based backend application built with Spring Boot, designed to manage employee data. This system includes features like adding, retrieving, updating, and deleting employee details and supports containerization with Docker.

---

## Features
- CRUD (Create, Read, Update, Delete) operations for employee data.
- RESTful API endpoints for seamless integration.
- Embedded H2 database for ease of use.
- Docker support for containerization.

---

## Prerequisites
To run this application, ensure you have the following installed:
1. **Java**: JDK 17 or higher.
2. **Maven**: For building and managing dependencies.
3. **Docker**: (Optional) For running the application in a container.

---

## Setup and Installation

### 1. Clone the Repository
```bash
git clone https://github.com/AarushGaikwad/EmployeeManagementSystem.git
cd EmployeeManagementSystem

2. Configure the Database
No additional setup is needed for the H2 database. The default configuration is already included in application.properties:

properties
Copy
Edit
spring.datasource.url=jdbc:h2:mem:employee_db
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true
To access the H2 database console:

Run the application.

Open your browser and navigate to http://localhost:8080/h2-console.

Use the following credentials:

JDBC URL: jdbc:h2:mem:employee_db

Username: sa

Password: (leave blank).

3. Build and Run the Application
Using Maven:

bash
Copy
Edit
mvn clean install
mvn spring-boot:run
