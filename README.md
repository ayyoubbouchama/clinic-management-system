@'
# Clinic Management System

A desktop application for managing clinic operations, built with Python.

## Technology Stack

- Python and PySide6 — desktop client
- FastAPI — centralized API backend
- PostgreSQL — shared relational database
- SQLAlchemy — database ORM
- Alembic — database migrations
- pytest — automated testing

## Architecture

Desktop clients communicate with the FastAPI backend over the clinic
network. The backend validates requests, enforces permissions, and
accesses PostgreSQL. Desktop clients do not connect directly to PostgreSQL.

## Repository Structure

- `desktop/` — PySide6 desktop application
- `backend/` — FastAPI backend and database migrations
- `database/` — SQL scripts and database documentation
- `tests/` — unit, API, and integration tests
- `docs/` — project documentation and team charter

## Setup

1. Install Python and PostgreSQL.
2. Create and activate a virtual environment.
3. Install dependencies using `python -m pip install -r requirements.txt`.
4. Create a local `.env` file based on `.env.example`.
5. Configure PostgreSQL and initialize the database migrations.
6. Start the backend and desktop client using the development instructions.

## Team Process Charter

[Read the Team Process Charter](docs/Team-Process-Charter.pdf)
'@ | Set-Content -Encoding utf8 README.md