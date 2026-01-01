# Multi-Tenant SaaS Platform

This project is a fully dockerized Multi-Tenant SaaS application built using **Node.js, PostgreSQL, React, and Docker**.  
It supports **tenant isolation**, **role-based access control**, and **project & task management**.

The entire application (database, backend, frontend) starts automatically using **one command**.

---

##  Tech Stack

### Backend
- Node.js
- Express.js
- PostgreSQL
- JWT Authentication
- Role-Based Access Control (RBAC)

### Frontend
- React (Vite)
- Axios
- Role-based UI rendering

### Infrastructure
- Docker
- Docker Compose

---

##  How to Run the Project (MANDATORY)

### Prerequisites
Make sure the following are installed:
- Docker
- Docker Compose

---

### ▶️ Start the Application

From the **project root directory**, run:

```bash
docker-compose up -d
````

This single command will:

* Start PostgreSQL database
* Run backend migrations & seed data automatically
* Start backend API
* Start frontend application

⚠️ **No manual database setup is required.**

---

##  Access the Application

| Service      | URL                                                                  |
| ------------ | -------------------------------------------------------------------- |
| Frontend     | [http://localhost:3000](http://localhost:3000)                       |
| Backend API  | [http://localhost:5000](http://localhost:5000)                       |
| Health Check | [http://localhost:5000/api/health](http://localhost:5000/api/health) |

---

##  Authentication & Roles

The system supports the following roles:

* **super_admin** – Global system administrator
* **tenant_admin** – Tenant-level administrator
* **user** – Regular tenant user

Each tenant’s data is completely isolated from other tenants.

---

##  Core Features

* Tenant registration & login
* User management (RBAC enforced)
* Project management
* Task management
* Secure JWT authentication
* Multi-tenant data isolation
* Fully dockerized setup

---

##  Testing the Application

After starting the application:

1. Open the frontend in browser
2. Login using credentials from `submission.json`
3. Verify:

   * Tenant isolation
   * Role-based access
   * Project & task operations

---

##  Demo Video

A complete demo video showcasing:

* Architecture walkthrough
* Docker startup
* Multi-tenancy
* User, project, and task flows

👉 **YouTube link will be added here.**

---

## 📌 Notes for Evaluators

* The application is fully dockerized
* All services start with `docker-compose up -d`
* Database migrations and seed data load automatically
* No manual commands are required
