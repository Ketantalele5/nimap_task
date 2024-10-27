Nimap Task - Spring Boot Project

This Spring Boot project provides a simple solution for managing categories and products. It supports CRUD operations for both entities and demonstrates a one-to-many relationship between Category and Product. The application uses a MySQL database and exposes RESTful API endpoints for performing these operations.

Features
Create, update, delete, and view categories.
Create, update, delete, and view products.
One-to-many relationship between Category and Product.
Uses Spring Data JPA and Hibernate for database operations.
Configurable database connection settings.
Server-side pagination for fetching products.
Technologies Used
Java (JDK 11+)
Spring Boot
Spring Data JPA
MySQL
Hibernate
Maven
Prerequisites
Before running this project, make sure you have the following installed:

Java JDK 17
MySQL Server
Eclipse, IntelliJ IDEA, or any Java-supported IDE
Maven
Getting Started
Follow these steps to set up and run the project:

1. Clone the Repository
Download the ZIP file or clone the repository:

bash
git clone git@github.com:Ketantalele5/nimap_task.git
Extract the files if you downloaded the ZIP.

2. Open the Project in an IDE
Open the project in Eclipse, IntelliJ IDEA, or any other Java-supported IDE.

3. Configure the MySQL Database
Ensure that MySQL Server is running on your local machine. Create a new database named nimap_task:

sql
CREATE DATABASE nimap_task;
Open the src/main/resources/application.properties file and configure the database connection settings:

properties
spring.datasource.url=jdbc:mysql://localhost:3306/nimap_task
spring.datasource.username=root
spring.datasource.password=root
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
4. Run the Application
In your IDE, run the NimapTaskApplication.java file as a Java application. The server will start on port 8080 by default. You can access the API at http://localhost:8080/.

API Endpoints
Here are the RESTful API endpoints available in this project:

Category Endpoints
GET /api/categories - Retrieve all categories.
GET /api/categories/{id} - Retrieve a specific category by ID.
POST /api/categories - Create a new category.
PUT /api/categories/{id} - Update an existing category.
DELETE /api/categories/{id} - Delete a category.
Product Endpoints
GET /api/products - Retrieve all products.
GET /api/products/{id} - Retrieve a specific product by ID.
POST /api/products - Create a new product.
PUT /api/products/{id} - Update an existing product.
DELETE /api/products/{id} - Delete a product.
GET /api/products?page={page}&size={size} - Retrieve products with server-side pagination.
