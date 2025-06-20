# Invoice-Management
A invoice management application built with Spring Boot, and MySQL.

Tech Stack
Backend
Spring Boot (Java 21)
Spring Security
Spring Data JPA
MySQL 8.0
JWT Authentication
Project Structure

Invoice-Management/        
├── backend/           # Spring Boot backend application
└── database/          # Database scripts and schema
Prerequisites
Java 21
MySQL 8.0
Maven
Setup Instructions
Database Setup
Install MySQL 8.0
Create a database named invoice_db
Use the following credentials:
Username: root
Password: YourPassword
Run the schema script from database/init.sql
Backend Setup
Navigate to the backend directory:
cd backend
Build the project:
mvn clean install
Run the application:
mvn spring-boot:run
The backend will start on http://localhost:8080


API Documentation
Authentication Endpoints
POST /api/auth/signup - Register new user
POST /api/auth/login - User login
Invoice Endpoints (Protected)
GET /api/invoices - Get all invoices
POST /api/invoices - Create new invoice
PUT /api/invoices/{id} - Update invoice
DELETE /api/invoices/{id} - Delete invoice
Testing
Import the Postman collection from postman/Invoice_System.postman_collection.json to test the APIs.

Features
User authentication with JWT
Protected routes
Invoice CRUD operations
Responsive design
Form validation
Error handling
Security Features
JWT token-based authentication
Password encryption
Protected API endpoints
Secure session management