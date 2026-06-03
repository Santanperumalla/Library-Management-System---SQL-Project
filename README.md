# Library Management System - SQL Project

## Project Overview

The **Library Management System** is a SQL-based database project designed to manage the day-to-day operations of a library. It helps store and organize information related to books, members, authors, publishers, book issues, and returns.

This project demonstrates database design concepts including:

* Database Creation
* Table Creation
* Primary and Foreign Keys
* Constraints
* Data Insertion
* Joins
* Aggregate Functions
* Subqueries
* Views


---

## Objectives

* Maintain records of books available in the library.
* Track library members and their activities.
* Manage book issuing and return processes.
* Generate reports for library operations.
* Practice SQL database design and querying skills.

---

## Technologies Used

* SQL
* MySQL

---

## Database Structure

The project consists of the following tables:

| Table Name   | Description                     |
| ------------ | ------------------------------- |
| Books        | Stores book information         |
| Authors      | Stores author details           |
| Publishers   | Stores publisher information    |
| Members      | Stores library member details   |
| Issue_Books  | Records book issue transactions |
| Return_Books | Records returned books          |

> Note: Update the table names according to your SQL script.

---

## Entity Relationship Overview

Main Relationships:

* One Author → Many Books
* One Publisher → Many Books
* One Member → Many Issued Books
* One Book → Multiple Issue Records

---

## Features

### Book Management

* Add new books
* Update book information
* Delete books
* Search books

### Member Management

* Register new members
* Update member details
* View member records

### Issue & Return Management

* Issue books to members
* Return books
* Track issued books
* Check overdue books

### Reporting

* Available books report
* Issued books report
* Member activity report
* Book inventory report

---

## Sample Queries Included

### Find All Available Books

```sql
SELECT * FROM Books;
```

### Find Issued Books

```sql
SELECT *
FROM Issue_Books;
```

### Count Total Books

```sql
SELECT COUNT(*) AS Total_Books
FROM Books;
```

### Find Most Issued Books

```sql
SELECT Book_ID,
       COUNT(*) AS Issue_Count
FROM Issue_Books
GROUP BY Book_ID
ORDER BY Issue_Count DESC;
```

---

## SQL Concepts Demonstrated

* DDL Commands

  * CREATE
  * ALTER
  * DROP

* DML Commands

  * INSERT
  * UPDATE
  * DELETE

* DQL Commands

  * SELECT
  * WHERE
  * ORDER BY
  * GROUP BY
  * HAVING

* SQL Joins

  * INNER JOIN
  * LEFT JOIN
  * RIGHT JOIN

* Advanced SQL

  * Subqueries
  * Views

---

## Project Structure

```text
Library-Management-System/
│
├── Library_Management_System.sql
└── README.md
```

---

## How to Run

### Step 1: Clone Repository

```bash
git clone https://github.com/your-username/Library-Management-System.git
```

### Step 2: Open Database Tool

Use any SQL database tool such as:

* MySQL Workbench
* pgAdmin
* SQL Server Management Studio (SSMS)

### Step 3: Execute SQL Script

Open:

```text
Library_Management_System.sql
```

Execute the script to:

* Create Database
* Create Tables
* Insert Sample Data
* Run Queries

---

## Learning Outcomes

Through this project, you will gain experience in:

* Relational Database Design
* Database Normalization
* SQL Query Writing
* Data Integrity Management
* Real-World Database Development

---
