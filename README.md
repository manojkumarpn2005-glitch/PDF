# 🚀 SQL Queries Project (DML & DDL)

## 📌 Overview

This project contains a collection of **SQL queries** performed on a `Transport` dataset.
It demonstrates both **DML (Data Manipulation Language)** and **DDL (Data Definition Language)** operations with example queries and outputs.

📄 Reference file: 

---

## 🗂️ Dataset Used

The dataset contains transport-related information such as:

* Transport_ID
* Vehicle_Type
* Route
* Distance_km
* Fuel_Type
* Passengers
* Fare
* Date
* City

---

## 🔧 DML Queries (Data Manipulation)

### 1. Display First 5 Records

```sql
SELECT * FROM Transport LIMIT 5;
```

### 2. Show Records Where Fare > 100

```sql
SELECT * FROM Transport WHERE Fare > 100;
```

### 3. Total Passengers by Vehicle Type

```sql
SELECT Vehicle_Type, SUM(Passengers)
FROM Transport
GROUP BY Vehicle_Type;
```

### 4. Increase Fare by 10 for Bangalore

```sql
UPDATE Transport
SET Fare = Fare + 10
WHERE City = 'Bangalore';
```

### 5. Delete Records Where Passengers ≤ 50

```sql
DELETE FROM Transport
WHERE Passengers <= 50;
```

---

## 🏗️ DDL Queries (Data Definition)

### 1. Insert New Record

```sql
INSERT INTO Transport 
(Transport_ID, Vehicle_Type, Route, Distance_km, Fuel_Type, Passengers, Fare, Date, City)
VALUES 
(201, 'Bus', 'Z', 18, 'Diesel', 55, 25, '2026-02-01', 'Bangalore');
```

### 2. Display All Records

```sql
SELECT * FROM Transport;
```

### 3. Select Records with Fare > 150

```sql
SELECT * FROM Transport WHERE Fare > 150;
```

### 4. Update Fare for Bangalore

```sql
UPDATE Transport
SET Fare = Fare + 10
WHERE City = 'Bangalore';
```

### 5. Drop Table

```sql
DROP TABLE Transport;
```

---

## 📊 Tools Used

* SQL (Databricks SQL Editor)
* Database Tables
* Query Execution with Output Verification

---

## 🎯 Key Learnings

* Understanding DML operations: SELECT, UPDATE, DELETE
* Working with aggregation functions like `SUM()`
* Applying filtering using `WHERE`
* Grouping data using `GROUP BY`
* Performing DDL operations like INSERT and DROP

---

## 📎 How to Use

1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
```

2. Open your SQL environment (Databricks / MySQL / PostgreSQL)

3. Run the queries step by step

---

## ⭐ Author

Manoj Kumar

---

## 📌 Notes

* Screenshots of outputs are included in the project PDF.
* Queries are tested and verified.

---

✨ Feel free to fork, use, and improve this project!
