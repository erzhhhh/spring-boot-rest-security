# Spring Boot REST CRUD with Spring Data JPA

This project serves as a comprehensive example of building a robust, production-grade RESTful API using Spring Boot and Spring Data JPA.

It implements a clean, Layered Architecture (Controller-Service-Repository pattern), demonstrating best practices for separation of concerns, data handling, and business logic implementation in Java.




## 🚀 Overview

The application provides a full set of CRUD (Create, Read, Update, Delete) operations for managing resources (e.g., Employees). It uses standard HTTP methods and returns clean, structured JSON responses.

### Key Features

  - Layered Architecture: Clear separation between the Web Layer (Controller), Business Layer (Service), and Data Access Layer (Repository).
  - Spring Data JPA: Simplifies database interactions using Hibernate under the hood.
  - REST Best Practices: Uses standard HTTP verbs (GET, POST, PUT, DELETE) and status codes.
  - Standard JSON: Returns simple, predictable JSON objects (POJOs).




## 🛠 Tech Stack

  - Java (JDK 21)
  - Spring Boot
  - Spring Data JPA (Hibernate)
  - MySQL Database




## ▶️ Running the project

```json
./mvnw spring-boot:run
```




## 🏗 Architecture

The project is organized into distinct layers to ensure maintainability and scalability:

  - REST Controller: Handles incoming HTTP requests and maps them to the correct service methods.
  - Service Layer: Contains the business logic (validations, calculations, etc.) and acts as a bridge between the Controller and the DAO.
  - DAO / Repository: Extends JpaRepository to handle direct database operations without boilerplate SQL.



## 📝 API Endpoints

The API is accessible at http://localhost:8080. 
Below are the available endpoints:
  - GET/api/employees  - retrieve a list of all employees
  - GET/api/employees/{id} - retrieve a specific employee by ID
  - POST/api/employees - create a new employee
  - PUT/api/employees/{id} - update an existing employee
  - DELETE/api/employees/{id} - delete an employee


## 📄 API Documentation (Swagger)

This project includes interactive API documentation powered by Swagger.
You can explore and test all endpoints directly in the browser:

  - http://localhost:8080/swagger-ui/index.html
  - OpenAPI JSON: http://localhost:8080/v3/api-docs
