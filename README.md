# Learning SQL — Alan Beaulieu (O'Reilly)

SQL fundamentals study repo. Covers the language systematically — set theory, query processing, subqueries, constraints, indexes, transactions, and stored procedures.

## Databases

- **MySQL 9.7** — primary database for book examples, connected via DBeaver
- **Sakila** — MySQL sample database used for most examples from Chapter 3 onwards (DVD rental store)

## Progress

| Chapter | Topic | Status |
|---|---|---|
| 1 | A Little Background | Complete (read only) |
| 2 | Creating and Populating a Database | Complete |
| 3 | Query Primer | Not started |

## Chapter 2 — Creating and Populating a Database

Concepts covered:

- `CREATE DATABASE` / `USE`
- `CREATE TABLE` — data types: VARCHAR, CHAR, SMALLINT, INTEGER, DECIMAL, DATETIME, YEAR, ENUM
- Constraints: PRIMARY KEY, FOREIGN KEY, CHECK, AUTO_INCREMENT
- Composite primary keys
- `ALTER TABLE` — modifying column types, adding/dropping constraints
- `INSERT INTO` — with and without AUTO_INCREMENT, NULL for auto-generated keys, `NOW()`
- `SELECT` — specific columns, `WHERE`, `ORDER BY`
- `UPDATE` — single and multiple rows
- `DELETE` — with WHERE clause
- `DESCRIBE` — inspecting table structure
- `str_to_date` — parsing non-standard date formats
- Foreign key constraint enforcement
- ENUM constraint enforcement

## Project

Chapter 2 concepts were applied to a self-designed project: [netherlands-telecoms-db](https://github.com/mclaughlin-samuel/netherlands-telecoms-db) — a MySQL database modelling mobile network operators in the Netherlands.
