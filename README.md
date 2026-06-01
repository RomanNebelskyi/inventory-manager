# Storage Manager

Spring Boot inventory management application with item and order tracking using Hibernate ORM.

## Features

- **Item management** — CRUD operations for inventory items (name, price)
- **Order management** — create and track orders with multiple items
- **Persistence** — Hibernate with PostgreSQL (H2 for development)
- **Web UI** — Thymeleaf templates for frontend
- **REST API** — exception handling via `@ControllerAdvice`

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Spring Boot 2.5 |
| ORM | Hibernate 5 |
| Database | PostgreSQL / H2 |
| Templating | Thymeleaf, JSP |
| Build | Maven |
| Java | JDK 11 |
| Utilities | Lombok |

## Getting Started

```bash
git clone https://github.com/RomanNebelskyi/storage2.git
cd storage2
./mvnw spring-boot:run
```

Configure `src/main/resources/hibernate.cfg.xml` and `application.properties` with your database credentials.

## Project Structure

```
src/main/java/com/example/storage2/
├── config/        — Hibernate, Spring MVC, Dispatcher config
├── controller/    — ItemController, OrderController, exception handler
├── model/         — JPA entities (Item, Orders)
├── DAO/           — Data access objects
└── start/         — Application entry point
```
