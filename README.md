# Invoice Processing Automation

## Overview
Invoice Processing Automation is a full-stack web application designed to streamline the management of invoices. It allows users to create, view, and manage invoices efficiently through a user-friendly interface. This project is built using Spring Boot** for the backend and Reactfor the frontend.

---

## Features
- Add Invoices: Quickly create new invoices with relevant details.
- View Invoices: Browse all invoices in a structured format.
- Update & Delete: Modify or remove invoices as needed.
- Responsive UI: React frontend ensures smooth user experience across devices.
- REST API:Spring Boot backend provides secure and efficient endpoints.

---

## Technology Stack
- Frontend:* React, JavaScript, HTML, CSS
- Backend: Spring Boot, Java
- Database:PostgresSQL
- Version Control:Git & GitHub

---

## Prerequisites

Before you begin, ensure you have the following installed:

- **Java Development Kit (JDK):** Version 17 or later.
- **Node.js:** Version 14 or later.
- **npm:** Node package manager (usually comes with Node.js).
- **Docker:** Docker Desktop (or Docker Engine + Compose plugin).

---

## Getting Started

To get a local copy up and running, follow these simple steps.

### Backend Setup

1.  **Navigate to the project directory:**
    ```sh
    cd Invoice-_Automation
    ```
2.  **Start PostgreSQL in Docker:**
    ```sh
    docker compose up -d
    ```
3.  **Make the Maven wrapper executable:**
    ```sh
    chmod +x mvnw
    ```
4.  **Run the Spring Boot application:**
    ```sh
    ./mvnw spring-boot:run
    ```
    The backend server will start on `http://localhost:8080`.

### Run Entire Project with Docker

You can run PostgreSQL, backend, and frontend together:

```sh
docker compose up --build
```

Services:

- Frontend: `http://localhost:3000`
- Backend: `http://localhost:8080`
- PostgreSQL: `localhost:5432`

#### Database Configuration

The backend now reads PostgreSQL configuration from environment variables, with Docker-friendly defaults:

- `DB_HOST` (default: `localhost`)
- `DB_PORT` (default: `5432`)
- `DB_NAME` (default: `invoiceprocessingautomation`)
- `DB_USERNAME` (default: `postgres`)
- `DB_PASSWORD` (default: `postgres`)

To stop Docker services:

```sh
docker compose down
```

### Frontend Setup

1.  **Navigate to the frontend directory:**
    ```sh
    cd invoice-frontend
    ```
2.  **Install NPM packages:**
    ```sh
    npm install
    ```
3.  **Run the React application:**
    ```sh
    npm start
    ```
    The frontend development server will start on `http://localhost:3000`.
