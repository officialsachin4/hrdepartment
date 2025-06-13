# HR-Department-Management-System-Rest-API

The HR Department Management System is a Spring Boot application that provides functionalities to manage employee information, attendance records, department details, positions, and salaries within an organization.

---

## 📑 Table of Contents

* [Features](#features)
* [Technologies Used](#technologies-used)
* [Getting Started](#getting-started)
* [Usage](#usage)
* [API Endpoints](#api-endpoints)
* [Database Configuration](#database-configuration)
* [Build and Run](#build-and-run)

---

## ✅ Features

* **Employee Management**: Add, update, retrieve, and delete employee information including name, email, phone number, address, department, and position.
* **Attendance Tracking**: Record employee attendance with in-time and out-time stamps.
* **Department Management**: Manage organizational departments, including adding, updating, retrieving, and deleting department details.
* **Position Management**: Maintain different job positions available within the organization.
* **Salary Management**: Track salary details for various positions, including basic salary, allowances, and gross salary calculations.

---

## 🛠 Technologies Used

* Java 8
* Spring Boot 2.7.14
* Spring Data JPA
* MySQL
* ModelMapper
* Lombok
* Maven

---

## 🚀 Getting Started

1. Ensure Java 8 or higher is installed.
2. Set up a MySQL database.
3. Configure database credentials in `application.properties`.
4. Clone the repository.
5. Build and run the project using Maven.

---

## 📦 Usage

The system provides RESTful API endpoints to manage employees, attendance, departments, positions, and salaries.

---

## 🔗 API Endpoints

### 👤 Employee Management

* `GET /api/employees` — Get all employees
* `GET /api/employees/{id}` — Get employee by ID
* `POST /api/employees` — Add new employee
* `PUT /api/employees/{id}` — Update employee
* `DELETE /api/employees/{id}` — Delete employee

### ⏱ Attendance Tracking

* `GET /api/attendances` — Get all attendance records
* `GET /api/attendances/{id}` — Get attendance by ID
* `POST /api/attendances` — Add attendance record
* `PUT /api/attendances/{id}` — Update attendance record
* `DELETE /api/attendances/{id}` — Delete attendance record

### 🏢 Department Management

* `GET /api/departments` — Get all departments
* `GET /api/departments/{id}` — Get department by ID
* `POST /api/departments` — Add new department
* `PUT /api/departments/{id}` — Update department
* `DELETE /api/departments/{id}` — Delete department

### 📌 Position Management

* `GET /api/positions` — Get all positions
* `GET /api/positions/{id}` — Get position by ID
* `POST /api/positions` — Add new position
* `PUT /api/positions/{id}` — Update position
* `DELETE /api/positions/{id}` — Delete position

### 💰 Salary Management

* `GET /api/salaries` — Get all salaries
* `GET /api/salaries/{id}` — Get salary by ID
* `POST /api/salaries` — Add new salary record
* `PUT /api/salaries/{id}` — Update salary
* `DELETE /api/salaries/{id}` — Delete salary

---

## 🗄️ Database Configuration

In your `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
spring.datasource.username=your_database_username
spring.datasource.password=your_database_password
```

---

## 🧱 Build and Run

```bash
# Navigate to the project directory
cd your-project-directory

# Build the project
mvn clean install

# Run the application
mvn spring-boot:run
```

Access the Swagger UI at:
**[http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)**
