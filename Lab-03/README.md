# Lab 03 — Containerized MySQL and SQL Data Management

**Course:** SRT411 — Digital Data Analytics  
**Platform:** Ubuntu Server, VirtualBox, Docker, Portainer, MySQL Workbench  
**Evidence:** 23-page academic lab report (PDF to be uploaded separately)

## Overview
This lab introduces a virtualized Linux database environment and uses SQL to create, query, modify, and manage a sales database. It also covers data preparation and the Extract–Transform–Load (ETL) process.

## Tasks completed

### 1. Virtualization and container deployment
- Installed and ran **Ubuntu Server** using **VirtualBox**.
- Installed **Docker** and configured **Portainer** for container management.
- Ran **MySQL in a Docker container** and verified connectivity through **MySQL Workbench**.

### 2. Data cleaning and preparation
- Removed duplicate entries and standardized country values with Excel's `UPPER()` function.
- Used `TRIM()`, cell formatting, and Find & Replace to normalize text, data types, and inconsistent formatting before database analysis.

### 3. Database creation and SQL operations
- Created a MySQL database and a sales table with typed fields, then loaded and inserted sample records.
- Practised `SELECT`, `WHERE`, `INSERT INTO`, `UPDATE`, `DELETE`, `GROUP BY`, `ORDER BY`, and `NOT IN`.
- Demonstrated `LEFT JOIN`, `RIGHT JOIN`, `INNER JOIN`, and a full-outer-join equivalent composed from joins.
- Created an index and a reusable SQL view for sales reporting.

### 4. SQL automation and transaction control
- Created and called a **stored procedure** for country-level sales details.
- Configured a **BEFORE UPDATE trigger** to populate a `Last_Updated` field.
- Used **transactions**, **savepoints**, **ROLLBACK TO SAVEPOINT**, and **COMMIT**, observing changes before and after commit.

### 5. ETL concepts
Explained the **Extract, Transform, Load (ETL)** process and its relevance to data quality and downstream analytics. This section is conceptual; the report does not document a complete automated ETL pipeline.

## Skills demonstrated
**Ubuntu Linux · VirtualBox · Docker · Portainer · MySQL · MySQL Workbench · SQL Joins · Relational Databases · Views · Indexes · Stored Procedures · Triggers · Transaction Management · Data Cleaning · ETL Fundamentals**

## Documentation
The original 23-page report contains implementation screenshots, SQL examples, and explanations. Upload the PDF to this folder and link it here.

## Scope and limitations
This is a structured **academic database and infrastructure lab**, not a production database service or a demonstrated security incident-detection implementation. Full Docker configuration and independently executable SQL source files are not included in this repository.
