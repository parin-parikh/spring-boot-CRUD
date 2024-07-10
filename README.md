# Spring Boot CRUD API

This project is a simple RESTful API built using Spring Boot for managing customer data. It provides CRUD operations (Create, Read, Update, Delete) to manage customers.

## Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)

## Features
- Add a new customer
- Retrieve a list of customers
- Update an existing customer
- Delete a customer

## Prerequisites
- Java 11 or higher
- Maven
- An IDE (e.g., IntelliJ IDEA, Eclipse)

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/parin-parikh/spring-boot-example.git
    cd spring-boot-CRUD
    ```

2. Build the project using Maven:
    ```bash
    mvn clean install
    ```

3. Run the application:
    ```bash
    mvn spring-boot:run
    ```

## Usage
Once the application is running, you can interact with the API using tools like Postman.

## API Endpoints
### Get all customers
- **URL:** `/api/v1/customers`
- **Method:** `GET`
- **Description:** Retrieve a list of all customers.

### Add a new customer
- **URL:** `/api/v1/customers`
- **Method:** `POST`
- **Description:** Add a new customer.
- **Request Body:**
    ```json
    {
        "name": "John Doe",
        "email": "john.doe@example.com",
        "age": 30
    }
    ```

### Update a customer
- **URL:** `/api/v1/customers/{customerId}`
- **Method:** `PUT`
- **Description:** Update an existing customer.
- **Request Body:**
    ```json
    {
        "name": "Jane Doe",
        "email": "jane.doe@example.com",
        "age": 25
    }
    ```

### Delete a customer
- **URL:** `/api/v1/customers/{customerId}`
- **Method:** `DELETE`
- **Description:** Delete a customer by ID.
