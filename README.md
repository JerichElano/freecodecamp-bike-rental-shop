# 🚲 Bike Rental Shop

An interactive Bash terminal application built as part of the **freeCodeCamp Relational Database Certification**. This project simulates an automated bike rental management system that handles inventory availability, records customer details, tracks active rentals, and processes returns using a PostgreSQL database.

## 📁 Repository Contents

* `bike-shop.sh` - Bash shell script containing the core menu logic, SQL queries, interactive prompts, and data manipulation rules.
* `bike_rental.sql` - PostgreSQL database dump containing the complete schema (tables, sequences, foreign keys) and initial seed data.

## 🛠 Tech Stack

* **Database:** PostgreSQL
* **Scripting:** Bash
* **CLI Utilities:** `psql`, `sed`, Regular Expressions (Regex)

## 🚀 Key Features

* **Interactive CLI Menu:** Multi-screen terminal interface with input validation and conditional menu routing.
* **Dynamic Inventory Checks:** Query-driven availability filtering that dynamically updates active rental inventory.
* **Automated Customer Onboarding:** Automatically queries incoming phone numbers to detect returning customers or insert new customer records.
* **Relational Data Tracking:** Connects customer accounts to specific bike inventory rows via a dedicated `rentals` junction table.

## 💡 Key Learnings & Challenges

* **Regex Pattern Matching:** Validating user input using Bash regex operators (`=~ ^[0-9]+$`) to ensure invalid inputs are handled safely.
* **SQL Joins & Relational Data:** Combining `bikes`, `customers`, and `rentals` tables via `INNER JOIN` queries to track active, unreturned rentals per customer.
* **Stream Operations & Formatting:** Utilizing standard Unix tools like `sed` and `read` loops to clean up raw PostgreSQL query outputs before displaying them to the user.
