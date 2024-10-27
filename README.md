# Nimap Task

## Overview
This project is a Spring Boot application designed for managing categories and products with RESTful APIs. It includes functionality for CRUD operations on both categories and products, with a one-to-many relationship between them.

## Technologies Used
- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL

## Features
- **Category Management**: Create, Read, Update, and Delete categories.
- **Product Management**: Create, Read, Update, and Delete products associated with categories.
- **Server-Side Pagination**: Efficiently handle large datasets for products.
- **RESTful APIs**: Interact with the application via HTTP requests.

## Database Configuration
- **Database Name**: nimap_task
- **Username**: root
- **Password**: root

## API Endpoints
### Categories
- `GET /api/categories` - Retrieve all categories and GET category by Id
  http://localhost:8080/api/categories?page=3
   http://localhost:8080/api/categories/{di}
- `POST /api/categories` - Create a new category
  http://localhost:8080/api/categories
- `PUT /api/categories/{id}` - Update an existing category
  http://localhost:8080/api/categories/{di}
- `DELETE /api/categories/{id}` - Delete a category
  	http://localhost:8080/api/categories/{di}
### Products
- `GET /api/products` - Retrieve all products and GET product by Id
  http://localhost:8080/api/products?page=2
  http://localhost:8080/api/products/{di}
- `POST /api/products` - Create a new product
  http://localhost:8080/api/products
- `PUT /api/products/{id}` - Update an existing product
  http://localhost:8080/api/products/{di}
- `DELETE /api/products/{id}` - Delete a product
  http://localhost:8080/api/products/{di}

## How to Run the Project
1. Clone the repository: `git clone git@github.com:Ketantalele5/nimap_task.git`
2. Navigate to the project directory.
3. Run the application using your IDE or by executing `mvn spring-boot:run`.
4. Ensure your MySQL database is running and configured as specified above.

## Conclusion
This project showcases the effective use of Spring Boot for managing categories and products with robust CRUD operations, a well-defined one-to-many relationship, and server-side pagination. 
