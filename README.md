# Formula-1-2024-Database-Management-System
Formula 1 2024 season database system with data cleaning, transformation, and analytical queries using SQL.

📖 Overview

This project is a Database Management System (DBMS) built using SQL to manage and analyze data from the 2024 Formula 1 season.

It covers the complete pipeline of:

Data ingestion
Data cleaning
Data transformation
Analytical querying
Transaction management

The system is designed to simulate a real-world sports analytics database.

📂 Dataset

The project uses multiple datasets including:

Race calendar
Drivers information
Teams data
Race results
Qualifying & sprint results
Driver of the Day votes

All datasets are structured and processed into relational tables.

🛠️ Tech Stack
SQL (PostgreSQL)
CSV datasets
Relational Database Design
🧠 Key Features
1. Database Design
Creation of normalized relational tables
Use of primary keys and foreign keys
Separation of raw and cleaned data tables

Example:

drivers_raw → drivers
race_results_raw → race_results
2. Data Cleaning & Preprocessing
Removal of duplicates using CTID
Handling NULL values
Data type conversions (TEXT → DATE, TIME, NUMERIC)
Standardization of inconsistent values

Example:

Converting date formats
Cleaning lap times and positions
3. Data Transformation
Derived columns such as:
race_distance_miles
total_points (race + sprint)
age of drivers
Normalization of country and team names
Index creation for performance optimization
4. Data Integrity
Foreign key constraints between tables
Ensuring consistency across:
Drivers
Teams
Race results
5. Advanced SQL Queries

Includes real-world analytical queries such as:

Total points per driver
Average lap time per circuit
Team participation statistics
Top countries hosting races
Multi-table joins (INNER, LEFT, RIGHT, FULL, CROSS)
6. Transaction Management (ACID Properties)
Implementation of:
BEGIN, COMMIT, ROLLBACK
SAVEPOINT
Simulation of failure scenarios and rollback recovery
🧾 Database Schema

Key tables include:

calendar
drivers
teams
race_results
qualifying_results
sprint_results
dotd_votes

👉 Full schema available in:
📄

⚙️ How to Run
Import CSV files into your PostgreSQL database
Execute the SQL script:
psql -U username -d database_name -f Formula_1.sql
Run queries to explore insights
📊 Sample Queries
Total points per driver
Average fastest lap per circuit
Team participation count
Race + sprint combined performance
🎯 Learning Outcomes
Practical understanding of DBMS concepts
Data cleaning and preprocessing techniques
Advanced SQL query writing
Transaction management and ACID properties
Real-world data modeling
