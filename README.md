# Async CRUD API with FastAPI and PostgreSQL

## Overview

This project is a simple asynchronous CRUD (Create, Read, Update, Delete) API implemented with FastAPI, using PostgreSQL as the database. It utilizes SQLAlchemy for ORM (Object-Relational Mapping) and Alembic for managing database migrations.

## Features

- **Asynchronous operations**: Built with FastAPI for high performance.
- **CRUD functionality**: Create, read, update, and delete items.
- **Database migrations**: Managed with Alembic.

## Prerequisites

- Python 3.7+
- PostgreSQL installed and running
- Create a database named `dbname` and a user with access to it.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/my_project.git
    cd my_project
    ```

2. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

3. Update the `DATABASE_URL` in `app/database.py` with your database credentials.

## Database Migration

To create the initial database structure, run:

```bash
alembic init migrations
alembic revision --autogenerate -m "Initial migration"
alembic upgrade head
