# SQL-Practice-Problems-SQL-Server-Solutions
SQL Practice Problems — SQL Server Solutions

Overview

This repository contains production-quality SQL Server solutions to the problems in SQL Practice Problems by Sylvia Moestl Vasilik.

It is not a dump of answers.
It is a curated record of analytical reasoning, defensive SQL patterns, and performance-aware query design — the kind required in real analytics and data engineering work.

The focus throughout is on:

Asking the right question

Choosing the correct data grain

Writing clear, correct, and maintainable SQL

Anticipating edge cases (NULLs, duplicates, datetime traps)

Thinking beyond syntax toward decision-ready insight

🎯 Purpose of This Repository

This repository exists to demonstrate:

How to reason with relational data under real-world constraints

How analytical SQL supports business decisions

How small design choices (joins, filters, grouping) materially affect results

How to write SQL that is readable, explainable, and performant

It is designed for:

Data Analysts

Data Engineers

BI Developers

Anyone who wants to move from writing SQL to thinking in SQL

🗂️ Repository Structure
sql-practice-problems-sql-server/
│
├── 01_introductory/
│   ├── 01_basic_selects.sql
│   ├── 02_filtering_where.sql
│   ├── 03_sorting_order_by.sql
│   ├── 04_string_numeric_functions.sql
│   ├── 05_date_handling.sql
│   └── README.md
│
├── 02_intermediate/
│   ├── 01_joins_and_relationships.sql
│   ├── 02_group_by_aggregates.sql
│   ├── 03_null_handling.sql
│   ├── 04_case_logic.sql
│   ├── 05_subqueries.sql
│   ├── 06_data_quality_checks.sql
│   └── README.md
│
├── 03_advanced/
│   ├── 01_window_functions.sql
│   ├── 02_ranking_and_partitioning.sql
│   ├── 03_time_series_analysis.sql
│   ├── 04_deduplication_patterns.sql
│   ├── 05_performance_optimization.sql
│   ├── 06_execution_plan_notes.sql
│   └── README.md
│
├── datasets/
│   └── northwind_modified_notes.md
│
├── diagrams/
│   ├── data_model.png
│   └── join_relationships.png
│
└── README.md

📚 Folder Breakdown
🟢 01_introductory/

Focuses on fundamentals done properly:

SELECT patterns with intent

Filtering and sorting without surprises

Date handling (date vs datetime)

String and numeric functions used correctly

Emphasis: clarity, correctness, and habit formation.

🟡 02_intermediate/

Introduces analytical thinking:

Multi-table joins and relationship reasoning

Aggregations and GROUP BY at the correct grain

NULL-aware logic

CASE expressions for business rules

Subqueries and validation checks

Emphasis: logic, assumptions, and data integrity.

🔴 03_advanced/

Deals with real-world complexity:

Window functions for ranking and comparison

Time-based analysis (periods, trends, rolling logic)

Deduplication and anomaly detection

Performance-aware query patterns

Execution plan considerations (SQL Server)

Emphasis: scalability, performance, and professional-grade SQL.

🧠 Coding Philosophy

Every SQL file follows these principles:

Queries are commented to explain intent, not just mechanics

Intermediate steps are preferred over clever one-liners

Defensive SQL is used where data may break assumptions

Readability is prioritized over brevity

Performance implications are acknowledged when relevant

Example comment style:

-- Aggregate at order level first to prevent join multiplication
-- before rolling up to customer grain

🧪 Database Used

The solutions are written for:

SQL Server

A modified Northwind-style database (as used in the book)

Note: These queries may require minor syntax adjustments for PostgreSQL or MySQL.

🚀 How to Use This Repository

Clone the repository

Open queries in SQL Server Management Studio (SSMS)

Run queries section by section

Read the comments before reading the results

Modify queries to test edge cases and assumptions

This repository is most valuable when used actively, not passively.

⚠️ Disclaimer

These solutions represent one correct and reasoned approach, not the only approach.
SQL is a language of trade-offs — and those trade-offs are documented where they matter.

💬 Final Thought

SQL doesn’t fail teams.
Thinking does.

If this repository helps sharpen how you think about data — it has done its job.
