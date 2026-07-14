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
| 4 | Filtering | Complete |
| 5 | Querying Multiple Tables | Complete |
| 6 | Working with Sets | Complete |
| 7 | Data Generation, Manipulation, and Conversion | Complete |
| 8 | Grouping and Aggregates | Complete |
| 9 | Subqueries | Complete |
| 10 | Joins Revisited | Complete |
| 11 | Conditional Logic | Complete |

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

## Chapter 4 — Filtering

Concepts covered:

- Condition types: equality, inequality, range (`BETWEEN`), membership (`IN`), pattern matching (`LIKE`)
- `NULL` conditions — `IS NULL`, `IS NOT NULL`
- `AND` / `OR` / `NOT` logic and operator precedence
- Subqueries in `WHERE` — using a SELECT result as a dynamic filter list
- `DELETE` with `WHERE` — row-level deletion and the importance of the WHERE clause

## Chapter 5 — Querying Multiple Tables

Concepts covered:

- `INNER JOIN` — joining two tables on a shared key
- Table aliases in multi-table queries
- Joining three or more tables
- Subqueries as a table source in `FROM`
- Cartesian product and why join conditions matter

## Chapter 6 — Working with Sets

Concepts covered:

- `UNION` — combining result sets, removing duplicates
- `UNION ALL` — combining result sets, keeping duplicates
- `INTERSECT` — rows common to both result sets
- `EXCEPT` — rows in the first result set not in the second
- Set operation rules — column count and data type compatibility
- Sorting combined result sets with `ORDER BY`

## Chapter 7 — Data Generation, Manipulation, and Conversion

Concepts covered:

- Working with temporal data — DATE, DATETIME, TIMESTAMP, YEAR
- Date formatting and parsing — `date()`, `time()`, `str_to_date()`, `date_format()`
- Date arithmetic — adding/subtracting intervals
- String functions — `concat()`, `length()`, `upper()`, `lower()`, `trim()`
- Numeric functions
- Type conversion

## Chapter 8 — Grouping and Aggregates

Concepts covered:

- `GROUP BY` — grouping rows by one or more columns
- Aggregate functions — `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`
- `HAVING` — filtering aggregated results
- Grouping by expressions
- `COUNT(*)` vs `COUNT(column)` and NULL behaviour

## Chapter 9 — Subqueries

Concepts covered:

- Subqueries in `WHERE`, `FROM`, and `SELECT` clauses
- Correlated vs non-correlated subqueries
- `EXISTS` / `NOT EXISTS`
- CTEs (`WITH` clause) — named subqueries for readability and reuse
- Cross joins and generating number series

## Chapter 10 — Joins Revisited

Concepts covered:

- `LEFT` / `RIGHT OUTER JOIN` — including unmatched rows
- `FULL OUTER JOIN`
- Self-joins
- Cross joins
- Natural joins

## Chapter 11 — Conditional Logic

Concepts covered:

- `CASE` expressions — simple and searched forms
- `CASE` in `SELECT`, `WHERE`, `ORDER BY`, and aggregations
- `CASE` with subqueries
- `COALESCE` and `NULLIF` as shorthand conditionals

## Project

Chapter 2 concepts were applied to a self-designed project: [netherlands-telecoms-db](https://github.com/mclaughlin-samuel/netherlands-telecoms-db) — a MySQL database modelling mobile network operators in the Netherlands.
