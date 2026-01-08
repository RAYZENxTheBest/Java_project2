# Java_project2


📌 Project Description

This project is a Spring Boot RESTful backend application designed to demonstrate fundamental CRUD (Create, Read, Update, Delete) operations on a Product entity.
The main objective of this project is to provide a clear understanding of:
1.REST API principles
2.Layered architecture in Spring Boot
3.DTO (Request / Response) usage
4.Exception handling
5.API documentation and testing using Swagger UI
This project is suitable for academic assignments, backend practice, and Spring Boot fundamentals learning.


🎯 Project Objectives

1.Implement RESTful endpoints following best practices
2.Separate concerns using controller, service, repository, and domain layers
3.Use DTOs to handle API requests and responses
4.Provide interactive API documentation via Swagger
5.Demonstrate clean and maintainable backend architecture


🧱 Technology Stack

1.Java 17+
2.Spring Boot
3.Spring Web
4.Spring Data JPA
5.Maven
6.Swagger / OpenAPI

🔗 Features - API Endpoints
Create – POST "/": Allows clients to create a product by sending product details in the request body. The createProduct method handles the operation and returns the created product as a response.

<img width="1419" height="286" alt="1" src="https://github.com/user-attachments/assets/ac443006-b503-4b71-a616-5f6fcafdf562" />


Get – GET "/{id}": Returns the product that matches the provided ID. If the product cannot be located, a ProductNotFound exception is raised.

<img width="1464" height="904" alt="2" src="https://github.com/user-attachments/assets/bc95043a-c3e3-4ae3-85ac-13df3d6dd129" />


Update – PUT "/{id}": Allows updating an existing product by supplying updated product information in the request body. The product is identified using its ID.

<img width="1064" height="934" alt="3" src="https://github.com/user-attachments/assets/c6184687-af52-42a3-9705-f8c17c73de7f" />

<img width="1094" height="377" alt="4" src="https://github.com/user-attachments/assets/9ff1c69d-6eae-4166-ae59-ccc212497b63" />


Get – GET "/": Retrieves a list of all available products stored in the system.Delete – DELETE "/{id}": Deletes a specific product identified by its ID from the database

<img width="1127" height="396" alt="5" src="https://github.com/user-attachments/assets/30e375e3-173f-4a76-a4eb-110c91140110" />


Delete – DELETE "/{id}": Deletes a product by ID and throws a ProductNotFound exception if the product is not found.

<img width="1107" height="581" alt="6" src="https://github.com/user-attachments/assets/dbc45584-6b93-41d3-951f-eebb49ab6d12" />

<img width="1124" height="697" alt="7" src="https://github.com/user-attachments/assets/dd14d45b-5616-49fc-9581-e4cf99c7112f" />


❌ Exception Handling

A ProductNotFoundException is thrown whenever the product ID provided does not match any existing product.

<img width="1125" height="700" alt="8" src="https://github.com/user-attachments/assets/eef64965-602c-424e-995b-96dba76aba8a" />

📄 Example JSON Request Bodies

Create - POST

{

"name" : "Example Product Name"

}

<img width="1090" height="231" alt="9" src="https://github.com/user-attachments/assets/ce8b1eeb-8bc0-4fdd-8dd7-deba0132b62d" />

Update - PUT

{

"name" : "New Product Name",

"id" : productID

}

<img width="1029" height="914" alt="10" src="https://github.com/user-attachments/assets/66a3f1a3-f42f-4efc-b30f-6d33423ff26d" />

<img width="1094" height="377" alt="11" src="https://github.com/user-attachments/assets/9b5e9285-06dc-46b8-a700-bc3862dde4fc" />

