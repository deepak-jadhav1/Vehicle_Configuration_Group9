# 🚗 Vehicle Configuration System

<div align="center">

### A Full-Stack Vehicle Configuration Platform

Configure vehicles, manage users, generate invoices, and process orders through a modern microservices-based architecture.

[![Java](https://img.shields.io/badge/Java-Spring%20Boot-orange?style=for-the-badge\&logo=openjdk)](https://www.java.com/)
[![.NET](https://img.shields.io/badge/.NET-ASP.NET%20Core-purple?style=for-the-badge\&logo=dotnet)](https://dotnet.microsoft.com/)
[![React](https://img.shields.io/badge/React-Frontend-blue?style=for-the-badge\&logo=react)](https://react.dev/)
[![MySQL](https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge\&logo=mysql)](https://www.mysql.com/)
[![Docker](https://img.shields.io/badge/Docker-Containerization-blue?style=for-the-badge\&logo=docker)](https://www.docker.com/)

</div>

---

## 📖 About The Project

The **Vehicle Configuration System** is a full-stack web application designed to provide users with an interactive platform for configuring and managing vehicles.

The system allows users to explore available vehicles, customize configurations, manage their accounts, place orders, and receive generated invoices and email notifications.

The project demonstrates a modern enterprise-style architecture by implementing the application using multiple technology stacks, including:

* ☕ **Java Spring Boot**
* 🔷 **ASP.NET Core (.NET)**
* ⚛️ **React.js**
* 🗄️ **MySQL**
* 🔐 **JWT Authentication**
* 🔑 **BCrypt Password Encryption**
* 🌐 **Google OAuth 2.0 / SSO**
* 📧 **Java and .NET Mail Microservices**
* 📄 **Invoice/PDF Generation**
* 🐳 **Docker & Docker Compose**
* 🔌 **RESTful APIs**

---

# ✨ Features

## 👤 User Management

* User Registration
* Secure Login
* JWT-based Authentication
* Password Encryption using BCrypt
* User Profile Management
* Role-based Access Control
* Secure Session Management

---

## 🔐 Authentication & Security

The application implements modern authentication and security mechanisms.

### Authentication Features

* JWT Token-based Authentication
* BCrypt Password Hashing
* Google OAuth 2.0 Authentication
* Secure API Access
* Protected Routes
* User Authorization

---

## 🚗 Vehicle Configuration

Users can configure vehicles based on available options and specifications.

Possible configuration options include:

* Vehicle Selection
* Model Selection
* Available Configurations
* Vehicle Features
* Custom Options
* Price Calculation

The system provides a flexible architecture for managing vehicle-related configurations.

---

## 🛒 Order Management

Users can manage their vehicle orders through the application.

Features include:

* Create Orders
* View Orders
* Manage Order Details
* Track Configured Vehicles
* Generate Order Information
* Maintain Customer Order Records

---

## 📄 Invoice Generation

The application supports invoice generation for vehicle orders.

Features include:

* Generate Invoice
* Create Order Summary
* Generate PDF Documents
* Maintain Invoice Details
* Send Invoice Information through Email

---

## 📧 Email Notification System

The project implements dedicated mail services using two different technology stacks.

### ☕ Java Mail Service

Implemented using:

* Spring Boot
* Spring Mail / JavaMail

### 🔷 .NET Mail Service

Implemented using:

* ASP.NET Core
* MailKit
* MimeKit

The mail services can be used for:

* Order Notifications
* Invoice Notifications
* User Communication
* Transactional Emails

---

# 🏗️ System Architecture

The project follows a distributed full-stack architecture.

```text
                         ┌───────────────────────┐
                         │       USER            │
                         └───────────┬───────────┘
                                     │
                                     ▼
                    ┌─────────────────────────────┐
                    │      REACT FRONTEND         │
                    │   Java / .NET Frontend      │
                    └──────────────┬──────────────┘
                                   │
                              REST APIs
                                   │
                 ┌─────────────────┴─────────────────┐
                 │                                   │
                 ▼                                   ▼
       ┌─────────────────────┐           ┌─────────────────────┐
       │   JAVA BACKEND      │           │    .NET BACKEND     │
       │   Spring Boot       │           │    ASP.NET Core     │
       └──────────┬──────────┘           └──────────┬──────────┘
                  │                                 │
                  └───────────────┬─────────────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │       MySQL         │
                       │      Database       │
                       └─────────────────────┘
                                  │
                 ┌────────────────┴────────────────┐
                 │                                 │
                 ▼                                 ▼
       ┌─────────────────────┐           ┌─────────────────────┐
       │ Java Mail Service   │           │ .NET Mail Service   │
       │ Spring Mail         │           │ MailKit / MimeKit   │
       └─────────────────────┘           └─────────────────────┘
```

---

# 🛠️ Technology Stack

## 🎨 Frontend

* React.js
* Vite
* JavaScript
* HTML5
* CSS3
* REST API Integration

---

## ☕ Java Backend

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* Spring Security
* Hibernate
* JWT Authentication
* BCrypt Password Encoding
* REST APIs

---

## 🔷 .NET Backend

* C#
* ASP.NET Core
* Entity Framework Core
* ASP.NET Core Web API
* JWT Authentication
* REST APIs

---

## 🗄️ Database

* MySQL
* Relational Database Design
* SQL Queries
* Database Initialization Scripts

---

## 📧 Email Services

### Java

* Spring Boot
* Spring Mail
* JavaMail

### .NET

* ASP.NET Core
* MailKit
* MimeKit

---

## 🔐 Security

* JWT Authentication
* BCrypt Password Hashing
* Google OAuth 2.0
* Protected APIs
* Secure Authentication Flow

---

## 🐳 DevOps & Deployment

* Docker
* Docker Compose
* Containerized Services

---

# 📂 Project Structure

```text
CDAC_PROJECT/
│
├── 📁 DotNetBackend/
│   └── ASP.NET Core Backend Application
│
├── 📁 DotNetVehicleMailService/
│   └── .NET-based Email Microservice
│
├── 📁 DotNet_Frontend/
│   └── React Frontend for .NET Backend
│
├── 📁 JavaBackend/
│   └── Spring Boot Backend Application
│
├── 📁 JavaVehicleMailService/
│   └── Java Spring Boot Email Microservice
│
├── 📁 Java_Frontend/
│   └── React Frontend for Java Backend
│
├── 📁 mysql-init/
│   └── MySQL Database Initialization Scripts
│
├── 📄 docker-compose-java.yml
│   └── Docker Configuration for Java Stack
│
├── 📄 docker-compose-dotnet.yml
│   └── Docker Configuration for .NET Stack
│
└── 📄 .gitignore
```

---

# 🔄 Application Workflow

The overall workflow of the application is as follows:

```text
1️⃣ User Opens Application
          │
          ▼
2️⃣ User Registers / Logs In
          │
          ▼
3️⃣ Authentication System Validates User
          │
          ▼
4️⃣ JWT Token is Generated
          │
          ▼
5️⃣ User Accesses Vehicle Configuration
          │
          ▼
6️⃣ User Selects Vehicle Options
          │
          ▼
7️⃣ Configuration and Pricing are Processed
          │
          ▼
8️⃣ User Places an Order
          │
          ▼
9️⃣ Order Details are Stored in MySQL
          │
          ▼
🔟 Invoice is Generated
          │
          ▼
📧 Email Notification is Sent
```

---

# 🔐 Authentication Flow

The system uses JWT-based authentication.

```text
User Login
    │
    ▼
Send Credentials
    │
    ▼
Backend Validates User
    │
    ▼
Password Verified Using BCrypt
    │
    ▼
JWT Token Generated
    │
    ▼
Token Sent to Frontend
    │
    ▼
Frontend Stores Token
    │
    ▼
Token Sent With Protected API Requests
    │
    ▼
Backend Validates JWT
    │
    ▼
Access Granted
```

---

# 🌐 REST API Architecture

The frontend communicates with the backend using RESTful APIs.

Typical API operations include:

| Method   | Description          |
| -------- | -------------------- |
| `GET`    | Retrieve Data        |
| `POST`   | Create New Data      |
| `PUT`    | Update Existing Data |
| `DELETE` | Delete Data          |

The APIs are responsible for handling:

* Authentication
* User Management
* Vehicle Management
* Vehicle Configuration
* Order Management
* Invoice Generation
* Email Communication

---

# 🗄️ Database

The application uses **MySQL** as the primary relational database.

The database is responsible for storing application data such as:

* Users
* Authentication Information
* Vehicles
* Vehicle Configurations
* Orders
* Customer Information
* Invoice Details

Database initialization scripts are available inside:

```text
mysql-init/
```

---

# 🐳 Docker Setup

The project provides separate Docker Compose configurations for the Java and .NET technology stacks.

## ☕ Run Java Stack

Navigate to the project directory and run:

```bash
docker-compose -f docker-compose-java.yml up --build
```

To run in detached mode:

```bash
docker-compose -f docker-compose-java.yml up -d --build
```

To stop the containers:

```bash
docker-compose -f docker-compose-java.yml down
```

---

## 🔷 Run .NET Stack

Run the .NET architecture using:

```bash
docker-compose -f docker-compose-dotnet.yml up --build
```

To run in detached mode:

```bash
docker-compose -f docker-compose-dotnet.yml up -d --build
```

To stop the containers:

```bash
docker-compose -f docker-compose-dotnet.yml down
```

---

# 🚀 Getting Started

## 📋 Prerequisites

Make sure the following software is installed on your system.

### Required Tools

* Java JDK
* Node.js
* npm
* MySQL
* Docker
* Docker Compose
* .NET SDK

---

# 💻 Running the Java Application

## Step 1: Clone the Repository

```bash
git clone https://github.com/deepak-jadhav1/Vehicle_Configuration_Group9.git
```

---

## Step 2: Navigate to the Project

```bash
cd Vehicle_Configuration_Group9/CDAC_PROJECT
```

---

## Step 3: Configure MySQL

Create and configure the required MySQL database.

Database initialization scripts can be found inside:

```text
mysql-init/
```

Update the database configuration in the backend configuration file according to your local MySQL setup.

Example configuration:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/your_database
spring.datasource.username=your_username
spring.datasource.password=your_password
```

---

## Step 4: Run Java Backend

Navigate to:

```bash
cd JavaBackend
```

Run the Spring Boot application using:

```bash
./mvnw spring-boot:run
```

Or:

```bash
mvn spring-boot:run
```

---

## Step 5: Run Java Mail Service

Navigate to:

```bash
cd JavaVehicleMailService
```

Run the application using:

```bash
mvn spring-boot:run
```

---

## Step 6: Run Java Frontend

Navigate to:

```bash
cd Java_Frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

---

# 🔷 Running the .NET Application

## Step 1: Navigate to .NET Backend

```bash
cd DotNetBackend
```

Restore dependencies:

```bash
dotnet restore
```

Run the application:

```bash
dotnet run
```

---

## Step 2: Run .NET Mail Service

Navigate to:

```bash
cd DotNetVehicleMailService
```

Restore dependencies:

```bash
dotnet restore
```

Run the service:

```bash
dotnet run
```

---

## Step 3: Run .NET Frontend

Navigate to:

```bash
cd DotNet_Frontend
```

Install dependencies:

```bash
npm install
```

Start the application:

```bash
npm run dev
```

---

# 📧 Email Configuration

The project uses email services for sending notifications and communication.

Before running the application, configure your email credentials securely using environment variables or application configuration.

⚠️ **Important:** Never commit sensitive credentials such as:

```text
Email Password
SMTP Password
JWT Secret
Database Password
OAuth Client Secret
API Keys
```

Instead, use:

* Environment Variables
* `.env` Files
* Docker Secrets
* Application Configuration

---

# 🔑 Environment Variables

A typical environment configuration may include:

```env
DB_HOST=localhost
DB_PORT=3306
DB_NAME=vehicle_db

DB_USERNAME=root
DB_PASSWORD=your_password

JWT_SECRET=your_jwt_secret

MAIL_USERNAME=your_email
MAIL_PASSWORD=your_email_password
```

> ⚠️ Never upload your `.env` file containing real credentials to GitHub.

---

# 📄 Invoice Generation

The application supports invoice generation for vehicle orders.

The invoice module can generate:

* Customer Details
* Vehicle Details
* Selected Configuration
* Order Information
* Pricing Details
* Invoice Summary

Invoices can be generated as PDF documents and shared with users through the email notification service.

---

# 🧩 Microservices

The application follows a modular architecture by separating responsibilities into different services.

## Main Services

### 🚗 Core Backend

Responsible for:

* Authentication
* Business Logic
* Vehicle Management
* Order Management
* Database Communication

---

### 📧 Mail Microservice

Responsible for:

* Sending Emails
* Order Notifications
* Invoice Notifications
* User Communication

---

### 🗄️ Database Service

Responsible for:

* Persistent Data Storage
* User Data
* Vehicle Data
* Order Data
* Configuration Data

---

# 🏛️ Architecture Pattern

The backend follows a layered architecture.

```text
Controller Layer
        │
        ▼
Service Layer
        │
        ▼
Repository / DAO Layer
        │
        ▼
Database Layer
```

### Controller Layer

Responsible for:

* Receiving HTTP Requests
* Returning HTTP Responses
* Calling Business Services

---

### Service Layer

Responsible for:

* Business Logic
* Application Rules
* Data Processing

---

### Repository Layer

Responsible for:

* Database Operations
* Data Persistence
* Query Execution

---

### Database Layer

Responsible for:

* Storing Application Data
* Maintaining Relationships
* Persistent Storage

---

# 🧪 Testing

Testing can be performed at different levels.

### Backend

* Unit Testing
* API Testing
* Integration Testing

### Frontend

* Component Testing
* API Integration Testing
* UI Testing

Recommended API testing tools:

* Postman
* Swagger / OpenAPI

---

# 📸 Screenshots

You can add application screenshots here.

## 🏠 Home Page

```text
📸 Add Screenshot Here
```

## 🔐 Login Page

```text
📸 Add Screenshot Here
```

## 🚗 Vehicle Configuration Page

```text
📸 Add Screenshot Here
```

## 🛒 Order Page

```text
📸 Add Screenshot Here
```

## 📄 Invoice

```text
📸 Add Screenshot Here
```

---

# 🚀 Future Enhancements

The following features can be added in future versions:

* [ ] Online Payment Integration
* [ ] Vehicle Comparison Feature
* [ ] AI-Based Vehicle Recommendation
* [ ] Advanced Search and Filtering
* [ ] Real-Time Order Tracking
* [ ] Admin Analytics Dashboard
* [ ] Cloud Deployment
* [ ] CI/CD Pipeline
* [ ] Kubernetes Deployment
* [ ] Mobile Application
* [ ] Multi-language Support
* [ ] Advanced Notification System

---

# 👥 Team

This project was developed as a **Group Project** as part of the CDAC program.

### Project Contributors

* **Deepak Jadhav**
* Group 9 Team Members

> Contributions and responsibilities were distributed among the project team members across frontend development, backend development, database management, integration, and deployment.

---

# 🎯 Learning Outcomes

Through this project, the team gained practical experience in:

* Full-Stack Web Development
* React.js Development
* Spring Boot Development
* ASP.NET Core Development
* RESTful API Development
* MySQL Database Design
* JWT Authentication
* OAuth Authentication
* BCrypt Password Security
* Microservices Architecture
* Email Service Integration
* PDF/Invoice Generation
* Docker Containerization
* Docker Compose
* Git and GitHub Collaboration

---

# 🤝 Contributing

Contributions are welcome.

To contribute:

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature/your-feature-name
```

3. Make your changes
4. Commit your changes

```bash
git commit -m "Add your feature"
```

5. Push the branch

```bash
git push origin feature/your-feature-name
```

6. Create a Pull Request

---

# 📜 License

This project is developed for **educational and academic purposes**.

---

# 👨‍💻 Author

**Deepak Jadhav**

* GitHub: https://github.com/deepak-jadhav1
* LinkedIn: https://www.linkedin.com/in/deepak-jadhav-780084228/

---

<div align="center">

### ⭐ If you found this project interesting, consider giving it a star!

**Built with ❤️ using Java, Spring Boot, .NET, React, MySQL, and Docker**

</div>
