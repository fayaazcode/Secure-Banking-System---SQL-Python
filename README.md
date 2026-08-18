# Secure-Database-Banking-System
This is a banking management program I did using Python and SQL for my class 12 board project.

The functions file has all the functions required for the main program to run

Banking system table creation has the SQL commands required to create the necessary tables with which the program runs


# Banking Management System

A robust, modular command-line Banking Management System built with **Python** and **MySQL**. Designed with production-level security practices, this application features cryptographic password hashing via `bcrypt`, parameterized database queries to prevent SQL injection, and explicit transactional integrity for financial operations.

---

## Key Features

* **Secure Authentication:** User passwords are encrypted using `bcrypt` salting and hashing before being stored in the database.
* **Defensive Database Engineering:** All database interactions use parameterized queries (`cursor.execute(query, params)`) to eliminate SQL injection risks.
* **Transactional Integrity:** Safe execution of financial operations (deposits, withdrawals, and inter-account fund transfers) utilizing explicit MySQL transaction commits.
* **Automated Audit Receipts:** Transaction history is tracked with auto-incrementing primary keys for real-time receipt generation and flexible filtering.
* **Modular Architecture:** Clean separation between the execution/driver script (`main.py`) and underlying database operations (`functions.py`).

---

## Tech Stack

* **Language:** Python 3.x
* **Database:** MySQL Server / MySQL Workbench
* **Database Connector:** `mysql-connector-python`
* **Security:** `bcrypt`

---

## Project Structure

```text
├── main.py                     # Primary execution/driver script for CLI interaction
├── functions.py                # Database queries, authentication, and core banking logic
├── schema.sql                  # DDL commands for database and table setup
├── .gitignore                  # Prevents environment variables and cache files from committing
└── README.md                   # Project documentation
```


This project was originally developed as a Class 12 CBSE Computer Science practical submission, demonstrating advanced database management, modular software design, and security fundamentals.
