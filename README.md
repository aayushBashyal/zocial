# Minimalist Task Management API with Authentication  
Built with **FastAPI**, **SQLAlchemy**, and **JWT Authentication**

---

## 🚀 Overview

This project is a clean and minimal backend API that provides:

- User **sign-up and login** with JWT authentication  
- Full **CRUD operations** for tasks  
- Integration with **SQLite** (local) or **PostgreSQL** (via Docker)
- Auto-generated **Swagger documentation** at `/docs`
- Environment-based configuration for easy deployment

It is ideal for learning backend fundamentals or presenting to clients as a demonstration of practical API development skills.

---

## 🧩 Features

### 🔐 Authentication
- User registration  
- Secure password hashing (Passlib)  
- JWT-based login and token refresh  
- Protected routes requiring authentication  

### 📝 Task Management
- Create a task  
- Read single or all tasks  
- Update a task  
- Delete a task  
- Each user manages *their own* tasks only  

### 🗄️ Database
- SQLite for local development  
- Optional PostgreSQL with Docker Compose  
- Uses SQLAlchemy ORM models and async session  

---

## 🛠️ Tech Stack

- **FastAPI** – high-performance Python web framework  
- **SQLAlchemy** – ORM for database interaction  
- **JWT (JSON Web Tokens)** – authorization  
- **Passlib** – password hashing  
- **Uvicorn** – ASGI server  
- **Docker + PostgreSQL** (optional)  

---

## 📁 Project Structure
app/
├── main.py
├── database.py
├── auth/
│ ├── models.py
│ ├── routes.py
│ └── utils.py
├── tasks/
│ ├── models.py
│ ├── routes.py
│ └── schemas.py
└── core/
├── config.py
└── security.py


---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
git clone https://github.com/your-username/minimalist-task-api.git
cd minimalist-task-api
