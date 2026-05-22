# Solar Energy SQL Analysis Project

## Overview
This project demonstrates practical SQL skills used in data analytics to analyze solar energy production and consumption data.

The project involved importing a relational database into MySQL using XAMPP and solving business-oriented analytical problems using SQL queries.

The dataset includes:
- Solar energy production
- Household energy consumption
- Battery usage
- Grid power transactions
- Weather conditions
- Sunlight duration

---

## Objectives
- Perform exploratory data analysis (EDA)
- Analyze energy production and consumption trends
- Evaluate battery and grid interactions
- Generate business insights using SQL

---

## Skills Demonstrated
- SQL Queries
- Joins
- Aggregate Functions
- Subqueries
- Stored Procedures
- UNION Operations
- Date & Time Functions
- Data Filtering and Sorting

---

## Tools Used
- MySQL
- XAMPP
- SQL

---

## Files Included

| File | Description |
|------|-------------|
| `solar.sql` | Database schema and solar energy dataset |
| `Code.txt` | SQL queries and analysis solutions |

---

## Database Tables

### `live_stats`
Contains time-series energy readings collected approximately every 5 minutes.

Key fields:
- Battery state of charge (`soc`)
- Grid power
- Consumption power
- Battery power
- Production power

---

### `daily_totals`
Contains aggregated daily energy statistics.

Key fields:
- Production
- Consumption
- Grid feed-in
- Energy purchased
- Charging energy
- Discharging energy

---

### `sunlight`
Contains sunrise, sunset, and total sunlight duration information.

---

### `weather`
Contains daily weather classifications such as:
- Sunny
- Rainy
- Partly cloudy

---

## Example Business Questions Solved
- Which days had above-average solar production?
- How does the weather impact battery charge levels?
- Which days purchased the most energy from the power grid?
- How much energy was sold back to the grid?
- What is the average nighttime battery charge?

---

## How to Load the Database

1. Open XAMPP and start:
   - Apache
   - MySQL

2. Open phpMyAdmin in your browser:

```text
http://localhost/phpmyadmin
```

3. Create a new database named:

```text
solar_db
```

4. Click the newly created database.

5. Open the **Import** tab.

6. Upload the `solar.sql` file and click **Go**.

The SQL file will automatically:
- Create tables
- Import data
- Build the database schema

---

## Example SQL Queries

### View all rows from daily totals

```sql
SELECT *
FROM daily_totals;
```

### View first 10 rows from live statistics

```sql
SELECT *
FROM live_stats
LIMIT 10;
```

### Count total records

```sql
SELECT COUNT(*)
FROM weather;
```

### View table structure

```sql
DESCRIBE daily_totals;
```

---

## Key Takeaways
This project strengthened my ability to:
- Work with relational databases
- Write analytical SQL queries
- Perform exploratory data analysis using SQL
- Generate insights from operational datasets

---

## Author
Vaibhav Magoo
