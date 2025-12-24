📘 SQL Practice Problems — SQL Server Solutions

🔍 Overview

This repository contains production-quality SQL Server solutions to the problems in
SQL Practice Problems by Sylvia Moestl Vasilik.

It is not a collection of copied answers.

It is a curated record of analytical reasoning, defensive SQL patterns, and performance-aware query design — the kind required in real analytics, BI, and data engineering work.

The emphasis throughout is on:

Asking the right questions

Choosing the correct data grain

Writing clear, correct, and maintainable SQL

Anticipating edge cases (NULLs, duplicates, datetime pitfalls)

Producing decision-ready insight, not just query output

🎯 Purpose

This repository exists to demonstrate how SQL is used in real environments to:

Reason with relational data under ambiguity

Translate business questions into analytical logic

Avoid silent data errors caused by poor joins, filters, or grouping

Write SQL that is explainable, testable, and scalable

It is intended for:

Data Analysts

Data Engineers

BI / Analytics Engineers

Anyone aiming to move from writing SQL to thinking in SQL

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
🟢 01_introductory

Foundations done properly

Focus areas:

Intentional SELECT statements

Filtering without surprises

Correct sorting and ordering

Date vs. datetime handling

String and numeric functions used safely

Emphasis: clarity, correctness, and habit formation.

🟡 02_intermediate

Analytical reasoning begins

Focus areas:

Multi-table joins and relationship logic

Aggregations at the correct grain

NULL-aware calculations

CASE expressions for business rules

Subqueries and data validation checks

Emphasis: logic, assumptions, and data integrity.

🔴 03_advanced

Real-world complexity

Focus areas:

Window functions and ranking logic

Time-based analysis and trends

Deduplication and anomaly detection

Performance-aware query design

Execution plan considerations (SQL Server)

Emphasis: scalability, performance, and professional rigor.

🧠 Coding Philosophy

Every SQL file follows consistent principles:

Queries are commented to explain intent, not just mechanics

Intermediate steps are preferred over clever one-liners

Defensive SQL is used where assumptions may break

Readability is prioritised over brevity

Performance implications are acknowledged where relevant

Example comment style:

-- Aggregate at order level first to prevent join multiplication
-- before rolling up to the customer grain

🧪 Database Used

SQL Server

A modified Northwind-style database (as used in the book)

⚠️ Note: Queries may require minor syntax adjustments for PostgreSQL or MySQL.

🚀 How to Use This Repository

Clone the repository

Open scripts in SQL Server Management Studio (SSMS)

Run queries section by section

Read the comments before reviewing results

Modify queries to test assumptions and edge cases

This repository delivers the most value when used actively, not passively.

⚠️ Disclaimer

These solutions represent one reasoned approach, not the only possible approach.

SQL is a language of trade-offs — and where those trade-offs matter, they are documented.

💬 Final Thought

SQL doesn’t fail teams.
Thinking does.

If this repository sharpens how you reason about data,
then it has done its job.
