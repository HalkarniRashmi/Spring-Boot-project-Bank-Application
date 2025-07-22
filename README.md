# Bank Account Management System

This project is a **RESTful web application** developed using **Java 21**, **Spring Boot**, and **MySQL**. It simulates core banking operations, including **Create**, **Read**, **Update**, and **Delete** (CRUD) functionality for bank accounts.

---

## 🔍 Problem Statement

**Title:** Bank Account Management System using Spring Boot

**Objective:**  
To develop a Spring Boot application that allows users to manage bank accounts through a REST API. Users can create, retrieve, update, and delete account details.

**Technologies Used:**  
- Java 21  
- Spring Boot  
- MySQL  
- Spring Data JPA  
- Postman  
- Swagger  

**Description:**  
The project models essential banking features with a modular, layered architecture for easier testing, maintenance, and scalability.

---

## 🧠 Architecture (UML Overview)

The system follows the **Controller → Service → Repository → Model** structure:

- **Model:** `BankAccount` – Defines entity structure.  
- **Repository:** `BankAccountRepository` – Interface extending `JpaRepository`.  
- **Service:** `BankAccountService` – Contains business logic.  
- **Controller:** `BankAccountController` – Exposes REST endpoints.  

---

## 📁 Project Structure
com.example.BankProject
│
├── Controller
│ └── BankAccountController.java
│
├── Service
│ └── BankAccountService.java
│
├── Repository
│ └── BankAccountRepository.java
│
├── Model
│ └── BankAccount.java
│
├── BankProjectApplication.java
└── BankProjectApplicationTests.java

yaml
Copy
Edit

---

## 🚀 Endpoints

| Method | Endpoint                  | Description                  |
|--------|---------------------------|------------------------------|
| GET    | `/api/accounts`           | Get all accounts             |
| GET    | `/api/accounts/{id}`      | Get account by ID            |
| POST   | `/api/accounts`           | Create a new account         |
| PUT    | `/api/accounts/{id}`      | Update an account by ID      |
| DELETE | `/api/accounts/{id}`      | Delete an account by ID      |

---

## 📦 Sample JSON Payload

### ➕ Create Account (POST)
```json
{
  "accountHolderName": "John Doe",
  "accountType": "Savings",
  "balance": 5000
}
🔁 Update Account (PUT)
json
Copy
Edit
{
  "accountHolderName": "Jane Doe",
  "accountType": "Current",
  "balance": 7500
}
✅ Testing Tools
Postman: Used for sending HTTP requests.

Swagger: Auto-generated API documentation and testing interface.

JUnit + SpringBootTest: For verifying application context and stability.

🛠️ How to Run
Clone the repo

Configure application.properties with your MySQL credentials

Run BankProjectApplication.java

Test APIs using Postman or Swagger at http://localhost:8080/swagger-ui.html



