# Authentication Simulation

A modern authentication system simulation built to demonstrate secure user authentication, authorization, and account management using a clean, scalable architecture.

> **Status:** Planning / Architecture Phase

---

# Overview

This project is designed to simulate how a production authentication service works while keeping the codebase educational, modular, and maintainable.

The project separates responsibilities into:

- React frontend
- FastAPI backend
- PostgreSQL database

The goal is to build an authentication service that follows industry best practices instead of creating a simple login form.

---

# Tech Stack

## Frontend

- React
- React Router
- Axios
- React Hook Form
- Zod
- TanStack Query

## Backend

- Python 3.12+
- FastAPI
- SQLAlchemy 2.x
- Alembic
- Pydantic v2
- JWT Authentication
- Passlib (bcrypt/argon2)
- Python-JOSE
- PostgreSQL Driver

## Database

- PostgreSQL

---

# Planned Features

## Authentication

- User Registration
- User Login
- User Logout
- Refresh Tokens
- JWT Authentication
- Remember Me
- Session Management

## User Account

- Email Verification
- Forgot Password
- Reset Password
- Change Password
- Update Profile
- Delete Account

## Security

- Password Hashing
- Rate Limiting
- Token Revocation
- Secure Cookies
- CSRF Protection (when applicable)
- CORS Configuration
- Input Validation
- SQL Injection Protection

## Administration

- User Roles
- Permissions
- Account Status
- User Management

---

# Installation

## Backend

```bash
cd backend

python -m venv .venv

source .venv/bin/activate
# Windows
# .venv\Scripts\activate

pip install -r requirements.txt
```

Run

```bash
uvicorn app.main:app --reload
```

---

## Frontend

```bash
cd frontend

npm install

npm run dev
```

---

# Coding Principles

- Keep business logic inside Services.
- Routers should only handle HTTP requests and responses.
- Database access belongs in Repositories.
- Use dependency injection where appropriate.
- Validate all user input.
- Never store plaintext passwords.
- Keep functions focused on a single responsibility.
- Follow RESTful API conventions.

---

# Future Improvements

- OAuth Login (Google, GitHub)
- Two-Factor Authentication (2FA)
- Redis Session Storage
- Device Tracking
- Login History
- Account Lockout
- WebAuthn / Passkeys
- Docker Compose
- CI/CD Pipeline
- Kubernetes Deployment

---

# Learning Goals

This project aims to provide practical experience with:

- FastAPI application architecture
- Authentication and authorization
- JWT lifecycle management
- Secure password storage
- PostgreSQL database design
- API security best practices
- React authentication flow
- Clean project organization
- Production-ready backend patterns

---

# License

This project is licensed under the MIT License.