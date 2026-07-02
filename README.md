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
| 3 | Query Primer | Complete |

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

## Chapter 3 — Query Primer

Concepts covered:

- `SELECT` clause — column selection, column aliases, expressions, `DISTINCT`
- `FROM` clause — table aliases, subqueries in FROM
- `WHERE` clause — comparison operators, `AND`/`OR`/`NOT`, `IN`, `BETWEEN`, `LIKE`, `IS NULL`
- `GROUP BY` and `HAVING`
- `ORDER BY` — ascending/descending, sorting by expressions
- How queries are executed by the MySQL server — connections, query parsing, optimisation, result sets
- `date()` and `time()` functions for extracting date/time components
- `concat()` for string concatenation
- Subqueries in the SELECT and FROM clauses

## Project

Chapter 2 concepts were applied to a self-designed project: [netherlands-telecoms-db](https://github.com/mclaughlin-samuel/netherlands-telecoms-db) — a MySQL database modelling mobile network operators in the Netherlands.
