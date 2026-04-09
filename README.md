# The Complete SQL Bootcamp: Zero to Hero 🚀

This repository contains my progress, notes, and solutions for **The Complete SQL Bootcamp**. The goal of this project is to demonstrate proficiency in PostgreSQL, ranging from basic data retrieval to complex database schema design.

## 📌 Project Overview
The repository is structured to mirror the learning path of the bootcamp, focusing on real-world applications of SQL in data analysis and business intelligence.

## 🛠️ Key Skills Covered
* **Foundational Queries:** SELECT, DISTINCT, WHERE, and ORDER BY.
* **Advanced Filtering:** Using LIKE, ILIKE, and Logical Operators.
* **Aggregation & Grouping:** Mastery of SUM, AVG, COUNT, GROUP BY, and HAVING.
* **JOINS:** Inner, Outer, Left, and Right Joins to connect relational data.
* **Advanced Techniques:** Subqueries, Self-joins, and the CASE statement.
* **Database Management:** Creating databases, tables, and handling constraints (CHECK, NOT NULL, UNIQUE).
* **Data Manipulation:** INSERT, UPDATE, DELETE, and ALTER commands.

## 📂 Repository Structure
* `01_Assessment_Tests/`: Solutions to milestone challenges within the course.
* `02_Group_By_Exercises/`: Deep dives into aggregate functions.
* `03_Joins_Practice/`: Complex multi-table queries.
* `04_Final_Project/`: A comprehensive database design and query challenge.

## 📊 Sample Query
```sql
-- Example: Finding high-value customers with more than 30 transactions
SELECT customer_id, COUNT(payment_id) AS total_transactions
FROM payment
GROUP BY customer_id
HAVING COUNT(payment_id) >= 30
ORDER BY total_transactions DESC;
