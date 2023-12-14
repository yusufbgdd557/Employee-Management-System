
# Employee Management Project

## Introduction
This application serves as a demonstration of an employee management system designed for employers. It features essential CRUD (Create, Read, Update, Delete) operations to efficiently manage employee data.

## Technologies Used

- **Java 17**
- **Spring Boot 3.2.0**
- **Spring Data JPA**
- **PostgreSQL**

## Features

### 1. Create
- Add new employees to the system by providing necessary details such as first name, last name and contact information.

### 2. Read
- View a comprehensive list of all employees with their respective details.
- Retrieve individual employee information based on unique identifiers.

### 3. Update
- Modify existing employee records to reflect changes contact details, or other relevant information.

### 4. Delete
- Remove employees from the system when they are no longer part of the organization.

## Environment Configuration

This project uses the `spring-dotenv` library to manage environment variables, especially for securing sensitive information like database credentials. Ensure the following dependency is included in your project's `pom.xml` file:

```xml
<dependencies>
    <!-- Other dependencies... -->
    <dependency>
        <groupId>me.paulschwarz</groupId>
        <artifactId>spring-dotenv</artifactId>
        <version>2.5.4</version>
    </dependency>
</dependencies>
```

### Using `.env` files

For enhanced security, utilize a `.env` file in the project's root to store environment variables. The `spring-dotenv` library will automatically load these variables into your Spring Boot application.

Example `.env` file:

```plaintext
DB_URL=jdbc:postgresql://localhost:5432/your_db_name
DB_USERNAME=your_database_username
DB_PASSWORD=your_database_password
```

Ensure the `.env` file is added to your `.gitignore` to prevent exposing sensitive information in version control.

## Getting Started

1. Clone the project to your local machine.
2. Open the project in an IDE (IntelliJ IDEA, Eclipse, etc.).
3. Perform necessary configuration checks, such as verifying database configurations or any external dependencies.
4. Run the `Application.java` class to start the application.
5. Visit `http://localhost:8080/swagger-ui.html` in your browser to explore and test the API. (Alternatively, you can use Postman if you are familiar with it.)

Note : Include instructions on setting up and running the project, emphasizing the importance of configuring the `.env` file for database connections.

### Sample Application Properties

To help you get started, here is an example `application.properties` file:

```properties
spring.datasource.url=${env.DB_URL}
spring.datasource.username=${env.DB_USERNAME}
spring.datasource.password=${env.DB_PASSWORD}
# Other Spring Boot configurations...
```

Adjust the properties based on your specific database and project requirements.



### Project Screenshots

![AddEmployeePage](https://github.com/yusufbgdd557/Employee-Management-System-Backend/assets/45573977/81aa6263-b5c8-4717-808a-54ecad1d4f60)

![Add-Employee](https://github.com/yusufbgdd557/Employee-Management-System-Backend/assets/45573977/fc8c2084-e3ee-4f40-a879-686d8c54bd4c)

![MainPage](https://github.com/yusufbgdd557/Employee-Management-System-Backend/assets/45573977/6030b205-592f-466e-ba97-a1a3d38cb62b)

![DeleteProcess](https://github.com/yusufbgdd557/Employee-Management-System-Backend/assets/45573977/f7e92dcb-be1b-44ac-be65-95f92ea710e0)
