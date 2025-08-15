# Category_Product_1_M_and-_M_1
Create One-to-Many and Many-to-One mappings for Category and Product.

The Category-Product Management System is a Spring Boot-based application designed to demonstrate the practical implementation of relational database concepts using modern Java development frameworks.
In this project, we explore One-to-Many and Many-to-One mappings, where:
One Category can have multiple Products
One Product belongs to exactly one Category
The system is organized into a layered architecture:
Controller Layer: Handles incoming HTTP requests and routes them to appropriate service methods.
Service Layer: Contains business logic and manages data processing between controllers and repositories.
Repository Layer: Provides an abstraction layer over the database operations using Spring Data JPA.
Entity Layer: Models the database structure with Hibernate annotations.
This project is an excellent starting point for developers who wish to understand relational mappings, entity lifecycle management, and CRUD API development with Spring Boot. By separating business logic from data persistence and request handling, it ensures maintainability, scalability, and testability of the application.




# Category-Product Management System (Spring Boot)

## Overview
This project demonstrates the implementation of **One-to-Many** and **Many-to-One** relationships between `Category` and `Product` entities using **Spring Boot**, **Spring Data JPA**, and **Hibernate**.  
It serves as a complete CRUD (Create, Read, Update, Delete) example, where each category can have multiple products, and each product belongs to exactly one category.

---

## Features
- REST API endpoints for **Category** and **Product**
- One-to-Many mapping from `Category` to `Product`
- Many-to-One mapping from `Product` to `Category`
- Service layer for business logic
- Repository layer using Spring Data JPA
- Entity modeling with Hibernate annotations
- API endpoints testable via Postman

---

## Project Structure





src/main/java
│
├── com.example.demo
│ ├── DemoApplication.java
│
├── com.example.demo.controller
│ ├── CategoryController.java
│ ├── ProductController.java
│
├── com.example.demo.entity
│ ├── Category.java
│ ├── Product.java
│
├── com.example.demo.repository
│ ├── CategoryRepository.java
│ ├── ProductRepository.java
│
└── com.example.demo.service
├── CategoryService.java
├── ProductService.java

src/main/resources
├── static/
├── templates/
└── application.properties






**API Endpoints**

Category Endpoints

Method	Endpoint	Description
GET	/categories	Get all categories
GET	/categories/{id}	Get category by ID
POST	/categories	Create new category
PUT	/categories/{id}	Update category
DELETE	/categories/{id}	Delete category



**Product Endpoints**

Method	Endpoint	Description

GET	/products	Get all products
GET	/products/{id}	Get product by ID
POST	/products	Create new product
PUT	/products/{id}	Update product
DELETE	/products/{id}	Delete product


**Tech Stack**

Java 17
Spring Boot
Spring Data JPA
Hibernate
Maven
MySQL / H2 Database
Postman (for testing APIs)


**How to Run**
Clone the repository:

git clone <repository-url>


Navigate to the project folder:
cd demo



**Update database configuration in application.properties:**

spring.application.name=demo



spring.datasource.url=jdbc:mysql://localhost:3306/assi_category_product_db
spring.datasource.username=root
spring.datasource.password=

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true





**Run the application:**

mvn spring-boot:run


Test APIs using Postman.





**License**

This project is licensed under the MIT License - see the LICENSE file for details.
