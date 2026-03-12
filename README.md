# PIX Payment Transaction Engine

A robust Back-end REST API for managing financial transactions via PIX, integrated with the Efipay SDK. This project focuses on security, scalability, and real-world payment flows.

## Technologies
- **Java 17**
- **Spring Boot 3.4.3**
- **Spring Security & JWT** (Authentication and Authorization)
- **Spring Data JPA** (MySQL Integration)
- **Efipay SDK** (Real PIX integration)
- **Docker & Docker Compose**
- **Lombok** (Boilerplate reduction)

## Infrastructure
The project uses Docker to manage the database environment.
- **Database:** MySQL 8.0
- **Container Port:** 3307 (Mapped to avoid local 3306 conflicts)

## Security Features
- **JWT Token:** Secure stateless authentication.
- **Validation:** Strict input validation using Spring Validation.
- **Environment Variables:** Sensitive data (API Keys, Mail credentials) are managed via environment variables for production safety.

## How to Run
1. Clone the repository.
2. Spin up the database: `docker compose up -d`
3. Set your environment variables (`JWT_SECRET`, `MAIL_USER`, etc.).
4. Run the application via IntelliJ or `./mvnw spring-boot:run`

---
Developed by **Jotadevs**
