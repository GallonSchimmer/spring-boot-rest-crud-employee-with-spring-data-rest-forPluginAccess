# Spring Boot REST CRUD Demo with Spring Data REST

This project is a Spring Boot application designed to demonstrate CRUD operations using Spring Data REST. It simplifies the process of building RESTful web services. 
This project is part of the Udemy course by Chad Derby: [Spring Boot 3, Spring 6 & Hibernate for Beginners](https://www.udemy.com/course/spring-hibernate-tutorial/?couponCode=SEPTSTACK24B).

## Project Overview

The application automatically handles CRUD operations for an `Employee` entity mapped to a MySQL database table. It utilizes Spring Data JPA to abstract the data layer, and Spring Data REST to expose these operations as RESTful endpoints.

## Features

- **Spring Data JPA Integration**: Simplifies data access within the application.
- **Automatic REST API**: Spring Data REST provides default CRUD operations over HTTP.
- **Repository Abstraction**: Minimal coding effort required for the repository layer.
- **Pagination and Sorting**: Default support provided by Spring Data REST.

## Technical Stack

- **Spring Boot**: Framework for building stand-alone, production-grade Spring based Applications.
- **Spring Data REST**: Framework to easily build hypermedia-driven REST web services on top of Spring Data repositories.
- **Spring Data JPA**: Provides repository support for JPA.
- **MySQL**: Database for storing the data.
- **Maven**: Dependency management.

## Running the Application

### Prerequisites

- JDK 17
- Maven
- MySQL

### Setup Database

Ensure MySQL is running and create an `employee_directory` database, or use the provided SQL script to set up and populate the `employee` table with initial data.

### Clone and Run

```bash
git clone https://github.com/YourGitHubUsername/RepositoryName.git
cd RepositoryName
mvn spring-boot:run
```

Access the application via: http://localhost:8080/magic-api/employees

## Development

This project uses Maven for managing dependencies and building the application. The main dependencies are Spring Boot Starter Data JPA, Spring Boot Starter Data REST, and MySQL Connector Java.

## Repository Configuration

The `EmployeeRepository` extends `JpaRepository` and uses the `@RepositoryRestResource` annotation to expose CRUD operations on the `Employee` entity.

## Application Properties

Configuration settings for the datasource, JPA, and Spring Data REST are located in `src/main/resources/application.properties`.

## Contribute

Contributions are welcome. Please fork the repository and submit a pull request.

## License

This project is open-sourced under the MIT license.


### Explanation of README Sections

- **Project Overview**: Introduces the project and its connection to the Udemy course.
- **Features**: Highlights the key functionalities and frameworks used.
- **Technical Stack**: Lists the technologies and frameworks used in the project.
- **Running the Application**: Detailed steps to set up and run the project locally.
- **Development**: Information about development practices and tools used.
- **Repository Configuration**: Briefly describes how the repository layer is configured.
- **Application Properties**: Mentions where the application configurations are stored.
- **Contribute**: Encourages contributions to the project.
- **License**: Specifies the licensing of the project.

This README is designed to give any user, including those new to programming, a clear understanding of what the project does, how to set it up, and how to use it.
