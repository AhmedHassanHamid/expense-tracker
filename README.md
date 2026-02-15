# 💰 Expense Tracker (REST API)

A professional-grade Back-End API built with **Java** and **Spring Boot**. This project focuses on complex data relationships, business logic validation, and external API integration.

---

## 🎯 Project Focus
This is a **Headless/Back-End-only** project. Instead of a UI, it is designed to be consumed by professional API clients like **Postman** or **Insomnia**.

## 🛠 Tech Stack & Dependencies
* **Java 17+**
* **Spring Boot 4.0.2
* **Spring Data JPA**: For MySQL persistence.
* **Spring Validation**: For ensuring data integrity.
* **MySQL**: Primary relational database.
* **Lombok**: To maintain clean, boilerplate-free code.

---

## 🚀 Development Roadmap

### 🟦 Phase 1: Persistence & Data Modeling (The Foundation)
- [x] Initialize project with Spring Initializr.
- [ ] Configure `application.properties` for MySQL.
- [ ] Create `Category` Entity (id, name, type).
- [ ] Create `Expense` Entity with `@ManyToOne` mapping to Category.
- [ ] Implement `JpaRepository` for both.

### 🟨 Phase 2: REST Layer (The API Contract)
- [ ] Implement **DTO Pattern** (Data Transfer Objects) to decouple the Database from the API.
- [ ] Create `ExpenseController` with standard REST endpoints (`GET`, `POST`, `DELETE`).
- [ ] Create `CategoryController`.
- [ ] **Postman Integration:** Create a Postman Collection for testing.

### 🟩 Phase 3: Service Layer & Logic
- [ ] Implement `ExpenseService` to handle core business logic.
- [ ] Add **Global Exception Handling** using `@ControllerAdvice`.
- [ ] Add validation rules (e.g., prevent negative expense amounts).
- [ ] Logic: Prevent deleting a Category if it still has linked Expenses.

### 🟧 Phase 4: Advanced Backend Features
- [ ] **Currency Conversion:** Integrate a 3rd-party API to allow saving expenses in different currencies.
- [ ] **Query Customization:** Write custom JPQL queries to filter expenses by month or category.
- [ ] **Logging:** Implement `SLF4J` logging for better debugging.
