## Overview
The **Task Management System** is a RESTful web application designed to help users create, manage, and track tasks efficiently.
The goal is to build a backend service using **Spring Boot** that supports CRUD operations for tasks, user management, and basic status tracking.

---

## Objective
To design and implement a scalable, maintainable REST API that allows:
- Creating new tasks
- Viewing existing tasks
- Updating task details or status
- Deleting completed or obsolete tasks

---

## Functional Requirements

###  Task Operations
- **Create Task**
    - Endpoint: `POST /tasks`
    - Input: task title, description, due date, status (default: PENDING)
    - Output: created task details with unique ID.

- **View All Tasks**
    - Endpoint: `GET /tasks`
    - Output: list of all tasks.

- **View Task by ID**
    - Endpoint: `GET /tasks/{id}`
    - Output: task details for the given ID.

- **Update Task**
    - Endpoint: `PUT /tasks/{id}`
    - Input: updated fields (title, description, due date, or status)
    - Output: updated task details.

- **Delete Task**
    - Endpoint: `DELETE /tasks/{id}`
    - Output: confirmation of deletion.

---

##  Non-Functional Requirements
- The API should follow **RESTful principles**.
- Responses should use **JSON** format.
- Proper **validation** and **error handling** must be implemented.
- The system should be **modular and testable**, following Spring Boot best practices.

---

## Tech Stack
| Layer | Technology |
|-------|-------------|
| Language | Java 17 |
| Framework | Spring Boot |
| Build Tool | Gradle |
| Database | PostgreSQL |
| Testing | JUnit, Mockito |

---

##  Future Enhancements
- User authentication and authorisation (Spring Security)
- Task categorisation (labels/tags)
- Notifications for due dates
- Pagination and sorting for large datasets

---

##  Deliverable
A fully functional Spring Boot REST API project with endpoints for managing tasks, ready to be extended with advanced features in later stages.

---

##  Learning Outcomes
- Building REST APIs with Spring Boot
- Implementing CRUD operations
- Using annotations like `@RestController`, `@RequestMapping`, and `@Entity`
- Understanding request/response handling in JSON
- Integrating with databases using Spring Data JPA