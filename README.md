# Relational Database Projects (PostgreSQL)

This repository contains SQL database dump files created as part of the **freeCodeCamp Relational Database** certification. These projects demonstrate my foundational skills in designing, building, and managing relational databases using PostgreSQL.

## 📂 Projects Included

### 1. Celestial Bodies Database (`universe.sql`)
A comprehensive database modeling various astronomical objects in the universe. 
* **Key Features:** Contains 5 interconnected tables (`galaxy`, `star`, `planet`, `moon`, `comet`).
* **Concepts Applied:** 
  - Primary and Foreign Keys establishing one-to-many relationships.
  - Data types including `INT`, `VARCHAR`, `NUMERIC`, `BOOLEAN`, and `TEXT`.
  - Constraints such as `UNIQUE` and `NOT NULL`.

### 2. Students and Courses Database (`students.sql`)
A relational database designed to track students, their majors, and the courses they are taking.
* **Key Features:** Contains 4 tables (`students`, `majors`, `courses`, `majors_courses`).
* **Concepts Applied:**
  - Implementation of a **many-to-many** relationship using a junction table (`majors_courses`).
  - Auto-incrementing primary keys (`SERIAL` / `SEQUENCE`).
  - Populating tables with `INSERT INTO` commands.

## 🛠️ Technologies & Skills
* **Database Management System:** PostgreSQL
* **Tools:** `psql` (CLI interface), `pg_dump` (Database backup/restoration)
* **SQL Skills:** DDL (Data Definition Language) for structuring tables, DML (Data Manipulation Language) for inserting data, Relational Database Design.

## 🚀 How to Use / Restore the Databases

If you want to recreate these databases on your local PostgreSQL server, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/vadymnaumenko893/freecodecamp-sql-projects.git
   ```
   
2. Navigate to the project folder and log into PostgreSQL:
   ```bash
   psql -U postgres
   ```

3. Run the SQL scripts to rebuild the databases:
   ```bash
   \i universe.sql
   \i students.sql
   ```

**(Note: The scripts contain commands to drop existing databases with the same name and create fresh ones).**
