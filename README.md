# 📝 Task Management REST API

[![Java](https://img.shields.io/badge/Java-17-blue)](https://www.java.com/)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.2-green)](https://spring.io/projects/spring-boot)
[![Build](https://img.shields.io/badge/Build-Maven-orange)](https://maven.apache.org/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)
[![Swagger](https://img.shields.io/badge/Swagger-UI-brightgreen)](http://localhost:8080/swagger-ui.html)

A simple **CRUD REST API** for managing tasks, built with **Java 17** and **Spring Boot**.  
Part of my **software architect portfolio**.

---

## 🚀 Features

- Create, read, update, delete tasks
- Mark tasks as completed
- Automatic task creation date
- Optional completion date
- API documentation with Swagger/OpenAPI
- Unit and integration tests included

---

## 📂 Project Structure

src/main/java/com/portfolio/tasks/
├─ controller/ → REST endpoints
├─ service/ → Business logic
├─ repository/ → JPA repositories
├─ model/ → Entities
├─ dto/ → Data Transfer Objects (optional)
└─ exception/ → Custom exception handling


---

## 🔌 Endpoints

| Method | Endpoint             | Description                    | Example Request Body |
|--------|--------------------|--------------------------------|-------------------|
| GET    | /tarefas            | List all tasks                 | -                 |
| GET    | /tarefas/{id}       | Get a task by ID               | -                 |
| POST   | /tarefas            | Create a new task              | `{ "titulo": "Task 1", "descricao": "Description" }` |
| PUT    | /tarefas/{id}       | Update a task                  | `{ "titulo": "Updated Task", "descricao": "Updated description", "concluida": false }` |
| DELETE | /tarefas/{id}       | Delete a task                  | -                 |
| PATCH  | /tarefas/{id}/done  | Mark task as completed         | -                 |

---

## 💻 How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ays78/task-management-api.git

2. **Navigate to the project folder**:
   ```bash
   cd task-management-api

3. **Build and run the application:**:
   ```bash
   mvn spring-boot:run

4. **Access API documentation at:**:
   ```bash
   http://localhost:8080/swagger-ui.html

🧪 Tests
Run all tests:
   ```bash
   mvn test

