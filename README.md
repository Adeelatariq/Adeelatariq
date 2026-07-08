# Tutoring Management System — Database Schema

A relational database schema for a **Tutoring Management System**, designed using an ERD (Entity Relationship Diagram) and EERD (Enhanced Entity Relationship Diagram), and translated into SQL.

## 📌 Overview

This project models the core entities and relationships involved in managing a tutoring service — connecting students with tutors, tracking parents, subjects taught, tutoring sessions, and session records.

The schema was designed by first mapping out entities and relationships in an ERD/EERD, then converting that design into a working SQL schema with tables, primary keys, foreign keys, and relationships.

## 🗂️ Entities / Tables

| Table | Description |
|-------|-------------|
| **Student** | Stores student information (e.g., name, contact details, grade level) |
| **Parent** | Stores parent/guardian information linked to one or more students |
| **Tutor** | Stores tutor information (e.g., name, contact, expertise) |
| **Subject** | Stores subjects offered for tutoring (e.g., Math, Physics, English) |
| **Session** | Represents a scheduled tutoring session, linking a student, tutor, and subject |
| **Record** | Stores records/outcomes of completed sessions (e.g., attendance, performance notes) |

## 🔗 Relationships

- A **Parent** can be linked to one or more **Students**.
- A **Student** can attend multiple **Sessions**.
- A **Tutor** can conduct multiple **Sessions**.
- Each **Session** is associated with one **Subject**.
- Each **Session** generates a corresponding **Record**.

## 🛠️ How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/Adeelatariq/Adeelatariq.git
   ```
2. Open the `schema.sql` file in your preferred SQL client (MySQL Workbench, pgAdmin, SQLite browser, etc.).
3. Run the script to create the database tables:
   ```bash
   mysql -u your_username -p your_database < schema.sql
   ```
   *(Adjust the command based on your database system — MySQL, PostgreSQL, SQLite, etc.)*

## 📁 Files

- `schema.sql` — Contains the full SQL schema (table definitions, keys, and relationships) derived from the ERD/EERD design.

## 📖 Design Process

1. **ERD** — Mapped out the basic entities (Student, Parent, Tutor, Subject, Session, Record) and their relationships.
2. **EERD** — Refined the design with additional constraints, keys, and relationship details.
3. **SQL Conversion** — Translated the finalized EERD into SQL `CREATE TABLE` statements, including primary keys, foreign keys, and constraints.

## ✍️ Author

Created by [Adeelatariq](https://github.com/Adeelatariq)
