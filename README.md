# Enterprise Management API
Modular Business Management Backend built with Spring Boot & PostgreSQL

A backend system designed to manage core enterprise operations including customers, suppliers, inventory, contracts, and service execution.

Built following layered architecture principles with REST APIs and relational database modeling.

---

## 🚀 Overview

Enterprise Management API is a Spring Boot application that provides a structured backend for managing business entities and operational workflows.

The system supports:

- Customer and supplier management
- Employee registry
- Inventory control and stock movements
- Purchase order processing
- Service execution tracking
- Contract management

Designed to simulate a real-world enterprise backend environment with relational modeling and business rule validation.

---

## 🏗 Architecture

The application follows a layered architecture:

- **Controller Layer** – REST endpoints
- **Service Layer** – Business rules and validation
- **Repository Layer** – Data access via Spring Data JPA
- **Persistence Layer** – PostgreSQL relational database

Entity relationships include:

- One-to-many
- Many-to-many
- Foreign key constraints
- Transactional consistency

---

## 🧱 Tech Stack

- **Java 18**
- **Spring Boot 3.4.4**
- **Spring Data JPA**
- **PostgreSQL**
- **Maven**
- **Docker (optional)**
- **JUnit (basic testing)**

---

## 📊 Core Features

- Full CRUD operations for all entities
- Relational database modeling
- Inventory movement tracking with referential integrity
- Service execution lifecycle management
- Contract association with customers
- Transactional operations using Spring

---

## 📂 Project Structure

```

src/
├── main/java/com/mateus/empresa_crud
│    ├── controller/
│    ├── service/
│    ├── repository/
│    ├── model/
│    └── config/
└── resources/
├── static/
└── application.properties

````

---

## 🗄 Database Design

The system uses PostgreSQL with:

- Primary keys
- Foreign key constraints
- Join tables for many-to-many relationships
- Automatic schema update via Hibernate

---

## ⚙️ Running the Application

### Requirements

- Java 17+
- PostgreSQL
- Maven

### Clone the repository

```bash
git clone https://github.com/mateuscardososs/enterprise-management-api.git
cd enterprise-management-api
````

### Configure database

Update `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/database_name
spring.datasource.username=username
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
```

### Run application

```bash
./mvnw spring-boot:run
```

Or run the main class in your IDE.

---

## 🐳 Running with Docker

```bash
docker compose up --build
```

---

## 📌 Engineering Concepts Demonstrated

* Layered architecture
* REST API design
* Relational database modeling
* Transaction management
* Separation of concerns
* Dependency injection
* Modular backend structure

---

## 📈 Possible Extensions

* JWT authentication
* Role-based access control
* Pagination and filtering
* OpenAPI documentation
* CI/CD pipeline
* Production-ready logging

---

## 👨‍💻 Author

Mateus Cardoso
Backend & Data-Driven Systems Engineer

```
