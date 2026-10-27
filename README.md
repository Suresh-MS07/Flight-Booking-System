# ✈️ Flight Booking System — Microservices Architecture

This project is a scalable, production-grade **Flight Booking System** built using a **microservices architecture**. It simulates real-world airline operations with modular, decoupled services for managing flights, bookings, API access, and user notifications.

---

## 📌 Overview

Each core domain is developed as an independent service:

| Service | Description |
| :--- | :--- |
| ✈️ **[Flight Service](./Flight-Service)** | Manages airports, cities, flights, and seat availability. |
| 📥 **[Booking Service](./Flight-Booking-Service)** | Handles user bookings, payment timeouts, and publishes events. |
| 🚪 **[API Gateway](./Flight-API-Gateway)** | Central entry point with authentication, rate limiting, and routing. |
| 📧 **[Notification Service](./Flights-Notification-Service)** | Sends email confirmations using RabbitMQ consumers. |

---

## 🧠 Key Features

- Microservices architecture using Node.js and Express
- REST APIs with modular MVC structure and Sequelize ORM
- JWT-based authentication with role-based authorization
- Asynchronous messaging with RabbitMQ
- Scheduled jobs (auto-cancel unpaid bookings)
- Email notifications using Node Mailer
- Docker-ready setup for containerized deployment

---

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MySQL (via Sequelize)
- **Messaging Queue**: RabbitMQ
- **Authentication**: JWT (access & refresh tokens)
- **Scheduler**: Node-Cron
- **Email**: NodeMailer
- **DevOps**: Docker, Postman for API testing

---

## 🚀 Getting Started

Each service is deployed separately. Follow the setup instructions below:

1. Clone the repository along with submodules:
   ```bash
   git clone --recursive <repository-url>
   cd Flight-Booking-System
