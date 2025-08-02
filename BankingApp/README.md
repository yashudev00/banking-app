# 🏦 SafeBank (Enterprise Digital Banking System)

An enterprise-grade digital banking platform built with **Java 17**, **Spring Boot**, **Spring Security (JWT)**, **JPA/Hibernate**, and **MySQL**. Supports secure user accounts, fund transfers, transaction history, audit logs, and role-based access control.

---

## 🚀 Key Features

- **User Registration & Login** using JWT-based authentication
- **Role-Based Access**: Admin, Manager, Customer (many‑to‑many mapping)
- **Account Management**: Create, view, and maintain bank accounts
- **Funds Transfer**: Internal transfer between accounts
- **Transaction History**: View past transactions with pagination & filtering
- **Audit Logs**: Record critical operations for traceability
- **Secure Password Hashing** with BCrypt
- **RESTful APIs** with standard status codes
- **Postman Collection** for testing endpoints

*(Future Enhancements)*: Docker containerization, admin dashboards, automated notifications

---

## 🛠️ Tech Stack

| Layer        | Technology / Tool                 |
|--------------|----------------------------------|
| Language     | Java 17                          |
| Framework    | Spring Boot 3.x, Spring Security |
| Persistence  | Spring Data JPA (Hibernate)      |
| Database     | MySQL                            |
| Auth         | JWT, BCrypt                      |
| Utilities    | Lombok (`@Builder`, etc.)        |
| API Testing  | Postman                          |
| Version Ctrl | Git / GitHub                     |

---

## 📁 Project Structure

```text
src
└─ main
   ├─ java
   │   └─ com.bankapp.BankingApp
   │       ├─ config         # Security, JWT, etc.
   │       ├─ controller     # REST endpoints
   │       ├─ dto            # DTO objects (requests & responses)
   │       ├─ model          # Entities: User, Role, Account, Transaction, Loan, etc.
   │       ├─ repository     # JPA repositories
   │       ├─ service        # Business logic & service layer
   │       └─ exception      # Custom exceptions & handlers
   └─ resources
       ├─ application.properties
       └─ data.sql (optional: seed data)

