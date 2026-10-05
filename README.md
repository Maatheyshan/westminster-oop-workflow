# Westminster OOP Module Workflow

[![Java](https://img.shields.io/badge/Java-17%2B-orange.svg)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)](https://spring.io/projects/spring-boot)
[![Build](https://img.shields.io/badge/Build-Maven-blue.svg)](https://maven.apache.org/)

Coursework project developed for the 2nd-year **Object-Oriented Programming (OOP) / Advanced Client-Server Architecture** module at the University of Westminster.

This repository implements a multi-tier client-server application utilizing Java Spring Boot, RESTful APIs, and fundamental OOP design patterns.

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Java
* **Framework:** Spring Boot
* **Modules:**
    * Spring Web (REST API endpoints)
    * Spring Data JPA (Object-Relational Mapping)
    * Lombok (Boilerplate code reduction)
* **Build Engine:** Maven

---

## 📐 Key OOP Concepts & Architecture

The application is structured into distinct layers to enforce separation of concerns and OOP principles:

* **Encapsulation:** Domain models use private fields with getter/setter access control and builder patterns.
* **Abstraction:** Business operations are abstracted behind interface contracts (e.g., `CourseService`, `UserService`).
* **Inheritance & Polymorphism:** Base entities leverage `@MappedSuperclass` or JPA inheritance strategies to extend common user and system behaviors.

### Directory Layout

```text
src/main/java/com/westminster/oop/
├── controller/     # Client REST Request Handlers
├── service/        # Business Logic Interfaces & Implementations
├── repository/     # Spring Data JPA Repositories
└── model/          # OOP Entities & Data Transfer Objects (DTOs)