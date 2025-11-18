# React + Tailwind + Flask Fullstack App

This project is a fullstack web application starter that uses:

- **React + Tailwind CSS** for a modern, responsive frontend
- **Flask (Python)** for a RESTful backend API
- A **relational database** (e.g. Postgres) for persistence
- Optional **Redis** and **Nginx** for caching and production deployment

It’s designed as a clean separation between **frontend** and **backend**, while staying simple enough to hack on quickly.

---

## Features

- 🔹 **SPA frontend** built with React (Vite or CRA) and Tailwind CSS  
- 🔹 **REST API** built with Flask and Blueprints (`/api/...`)  
- 🔹 **JWT authentication** (login, register, current user)  
- 🔹 **SQLAlchemy models + migrations** (via Flask-Migrate/Alembic)  
- 🔹 **CORS-aware** dev setup (frontend and backend on different ports)  
- 🔹 Structured, extensible project layout for both frontend and backend

---

## Tech Stack

**Frontend**

- React (SPA)
- Tailwind CSS
- React Router
- `fetch` or `axios` for API calls
- (Optional) React Query / TanStack Query for data fetching and caching

**Backend**

- Python + Flask
- Flask Blueprints (modular routing)
- SQLAlchemy (ORM)
- Flask-Migrate (database migrations)
- (Optional) flask-jwt-extended or Flask-Login for authentication
- (Optional) Redis for caching / sessions

**Database & Infra**

- Postgres (recommended) or SQLite for local development
- Nginx or similar reverse proxy in production
- Docker / container-based deployment (optional)

---

## High-Level Architecture

```text
[ React + Tailwind SPA ]  <---- HTTP/JSON ---->  [ Flask API ]
         |                                                |
         |                                                |
         └-----------------> [ Postgres / Redis ] <-------┘
