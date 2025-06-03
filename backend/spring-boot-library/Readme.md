# Spring Boot Backend - for Library

This is the backend service built with **Spring Boot** that powers the **React-based Library App**.  
It handles:


- REST API communication with the frontend
- Data processing and persistence
- Business logic and library operations

## 1. Backend Design

The Spring Boot backend includes the following Spring ecosystem components to provide a robust and concise implementation:

- **Lombok** – Reduces boilerplate code for models (getters, setters, constructors, etc.)
- **Spring Data JPA** – Simplifies database interactions using repository patterns
- **Spring Data REST** – Automatically exposes RESTful endpoints for repositories
- **MySQL Driver** – JDBC driver to connect the app with a MySQL database



## 2. Build and Run Application
## 2.1 Requirements
- **Java 17** installed and configured in your system.
- **MySQL Server** running on port `3306`.
- A MySQL user with the following credentials:
    - **Username**: `springstudent`
    - **Password**: `springstudent`

- Before running the application, the required database tables must be created and populated.

  - You can do this using the SQL scripts provided in: ``
/starter-files/Database-Scripts
``


## 4. Example of Using the Application

To use this application, follow the steps below:

### 4.1. Download the Application
Clone the repository to your local machine using Git:
```
git clone git@github.com:MarianVJ/priceComparatorBackend.git
```

### 4.2 Build the Application
To build the application, use the following Maven wrapper command:
```
./mvnw clean package
```



### 4.3 Run the application
This will start the Spring Boot application. By default, it should be accessible at `http://localhost:8080`.
```
./mvnw spring-boot:run
```
### 4.4 Features

Each feature has its own classes for Controller, Service, and Repository. This decision was made considering the possibility of extending the features with more complex or additional functionality.

#### Detail