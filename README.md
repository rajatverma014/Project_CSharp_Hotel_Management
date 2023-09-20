# Project_CSharp_Hotel_Management
This repository contains the source code and documentation for the XYZ Hotels API Core Project. This project is designed to streamline the reservation process and provide an efficient booking experience for XYZ Hotels' customers. It includes CRUD operations for managing hotel information, filtering capabilities, count functionality for room availability, JWT token authentication for secure access, and handles the one-to-many relationship between hotels and rooms.
Table of Contents
Project Overview
Objectives
Approach
Getting Started
API Endpoints
Authentication
Exception Handling
Database Schema
Contributing
License
Project Overview
XYZ Hotels is a renowned hotel chain operating globally. To meet their goals of providing an efficient booking experience and secure access to their reservation system, this API Core Project was developed. It includes comprehensive functionality such as CRUD operations for managing hotels, filtering hotels based on various criteria, counting available rooms, JWT token authentication, and handling the one-to-many relationship between hotels and rooms.

Objectives
CRUD Operations: Develop APIs for managing hotel information, including creating, updating, retrieving, and deleting hotels.
Filtering: Implement filtering capabilities to allow customers to search and filter hotels based on criteria such as location, price range, or amenities.
Count Functionality: Enable users to obtain counts of available rooms in specific hotels, providing insights into room availability.
JWT Token Authentication: Implement a secure authentication mechanism using JWT tokens to ensure only authorized users can access the API endpoints.
One-to-Many Relationship: Establish an efficient solution to handle the one-to-many relationship between hotels and rooms.
Exception Handling: Implement try-catch blocks to handle exceptions gracefully, providing meaningful error messages and ensuring system stability.
Repository Pattern: Apply the repository pattern to separate the data access layer from the business logic, promoting code modularity and maintainability.
Approach
Database Design: Define the database schema, including tables for hotels, rooms, and the necessary foreign key relationships.
Code-First Development: Employ a code-first approach to generate the database schema based on the defined models and relationships using frameworks like Entity Framework.
Repository Implementation: Implement repositories for hotels and rooms, following the repository pattern to handle data access operations.
CRUD Operations: Implement APIs to support creating, reading, updating, and deleting hotel information.
Filtering: Develop APIs that enable customers to search and filter hotels based on specified criteria.
Count Functionality: Implement APIs to provide counts of available rooms in specific hotels.
JWT Token Authentication: Integrate JWT token authentication to secure the API endpoints.
Exception Handling: Implement try-catch blocks to handle exceptions gracefully.
One-to-Many Relationship: Design and implement the necessary database mappings and APIs to handle the one-to-many relationship between hotels and rooms.
Getting Started
To get started with this project, follow these steps:

Clone the Repository: git clone <repository-url>
Install Dependencies: Run npm install to install the required packages.
Database Configuration: Configure your database connection in appsettings.json or .env file.
Run Migrations: Run dotnet ef database update to apply database migrations.
Start the Application: Run dotnet run to start the API server.
Access API Documentation: Visit http://localhost:5000/swagger for API documentation and usage details.
API Endpoints
The API provides the following endpoints:

POST /api/hotels: Create a new hotel.
GET /api/hotels/{id}: Retrieve hotel details by ID.
PUT /api/hotels/{id}: Update hotel details by ID.
DELETE /api/hotels/{id}: Delete a hotel by ID.
GET /api/hotels: Retrieve a list of hotels with optional filtering.
GET /api/hotels/{id}/rooms/count: Get the count of available rooms in a hotel.
POST /api/auth/login: Authenticate and obtain a JWT token.
POST /api/auth/register: Register a new user account.
For more detailed information and examples, refer to the API Documentation.

Authentication
This project uses JWT token authentication to secure API endpoints. To access protected resources, you must obtain a JWT token by authenticating using the /api/auth/login endpoint. Include the token in the Authorization header of your requests.
Exception Handling
The project includes robust exception handling with meaningful error messages. In case of an error, the API will return a JSON response with a status code and error details.

Database Schema
The database schema is generated using a code-first approach. Refer to the database model classes in the code for schema details.

Contributing
If you'd like to contribute to this project, please follow the standard Git flow:

Fork the repository.
Create a new branch for your feature or bug fix.
Make your changes and commit them.
Push your branch to your fork.
Create a pull request to the main repository's main branch.
