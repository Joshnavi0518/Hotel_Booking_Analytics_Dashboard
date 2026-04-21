# 🏨 Hotel Booking Analytics Dashboard using Snowflake SQL

## 📌 Project Overview
This project focuses on building a data analytics solution for hotel bookings using Snowflake SQL. The goal is to analyze booking patterns, revenue trends, customer behavior, and operational performance using curated gold-layer datasets.

The project simulates a real-world analytics pipeline where raw data is transformed into business-ready insights using SQL queries.

---

## 🎯 Objectives
- Calculate key business KPIs such as revenue, bookings, and guest count
- Analyze monthly trends in bookings and revenue
- Identify top-performing cities and room types
- Understand booking status distribution
- Build a SQL layer for dashboard visualization

---

## 🛠️ Tools & Technologies Used
- Snowflake (Data Warehouse)
- SQL (Data Analysis)
- Snowsight Worksheets
- GitHub (Version Control)

---

## 🗂️ Data Model
The project uses curated **Gold Layer tables**:

- `GOLD_BOOKING_CLEAN` → Cleaned booking-level data
- `GOLD_AGG_DAILY_BOOKING` → Daily aggregated metrics
- `GOLD_AGG_HOTEL_CITY_SALES` → City-wise revenue aggregation

---

## 📊 Key Performance Indicators (KPIs)

- **Total Revenue**
```sql
SELECT SUM(total_amount) AS total_revenue
FROM GOLD_BOOKING_CLEAN;
