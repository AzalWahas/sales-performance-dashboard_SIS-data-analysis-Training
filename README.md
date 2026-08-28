# 📊 Retail Sales Analysis & Interactive Dashboard (2024)

An interactive retail performance dashboard designed to track high-level sales metrics, analyze regional customer distributions, evaluate category trends, and monitor item-level revenue streams for 2024.

---
## 🚀 Project Overview

This repository documents the full lifecycle of building a retail analytics solution—from raw data extraction to dynamic data visualization. The dashboard tracks key business KPIs including revenue growth, unit sales volume, top-performing SKUs, and regional performance across five major product categories and key Egyptian metropolitan cities.

### Key Metrics Summary
* **Total Sales Revenue:** ~$6.98M
* **Total Units Sold:** 90,294 units
* **Top Selling SKU:** Doll Product ($522,606)

---
## 🗃️ Dataset Overview

The dataset covers retail transactions for 2024 and contains the following core fields:

* **`Order_Date`:** Transaction timestamp spanning January through December 2024.
* **`Customer_ID`:** Unique customer identifiers used to aggregate regional active user counts.
* **`City / Region`:** Key geographic locations (**Alexandria, Aswan, Cairo, Giza, Mansoura**).
* **`Category`:** Product classifications (**Toys, Clothing, Electronics, Furniture, Books**).
* **`Product`:** Specific item designations (*e.g., Doll, Puzzle, Shirt, Laptop, Novel*).
* **`Sales_Amount`:** Total monetary value generated per line item ($ USD).
* **`Units_Sold`:** Quantity of items purchased per transaction.

---

## ⚡ Dashboard Features

* **Executive KPI Summary:** Displays high-level business benchmarks including total sales revenue, total units sold, and the top-performing SKU.
* **Interactive Timeline Slicer:** Left-side timeline panel for dynamic filtering by specific months (Jan–Dec 2024).
* **Regional Analysis Chart:** A dual-axis column chart comparing customer volume (`Count of CustomerID`) against revenue generation (`Total Sales`) across 5 major Egyptian cities.
* **Category Distribution Donut Chart:** Shows proportional revenue contribution across all five primary product categories.
* **Sales Trend Line Chart:** Tracks continuous monthly revenue shifts in millions throughout 2024.
* **Granular Product Bar Chart:** Itemized revenue breakdown grouped by category to evaluate high vs. low performing inventory.

---

## 💡 Key Business Insights

1. **Overall Performance:** Generated **$6,977,094.80** in total sales with **90,294 units sold**. The **Doll Product** was the top-selling item, bringing in **$522,606**.
2. **Category Balance:** Revenue is evenly split across all categories: **Toys** leads at **20.46%**, followed by **Furniture** (20.20%), **Electronics** (20.07%), **Books** (19.73%), and **Clothing** (19.55%).
3. **Monthly Trends:** Sales trajectory peaks in **April** (exceeding $7.3M), followed by a steady run through mid-year and a dip around February ($6.8M range).
4. **Geographic Distribution:** Active customer count remains evenly balanced (56 to 62 customers per city), with **Aswan** and **Mansoura** demonstrating top sales volume relative to customer numbers.
5. **Product Performers:** Top category drivers include **Dolls, Puzzles, and Shirts**, while sub-items like **Sofas** and **Headphones** generated lower overall revenue.

## 🛠️ Project Stages & Workflow
<img width="790" height="100" alt="image" src="https://github.com/user-attachments/assets/5cf9b537-a053-447e-a317-125486d1b3f6" />

### Stage 1: Data Collection & Intake
* Gathered transactional records for 2024 containing dates, regions, customer IDs, product sub-categories, sales revenue, and quantities sold.
* Schema mapping across 5 core product categories: **Toys, Furniture, Electronics, Clothing, and Books**.

### Stage 2: Data Cleaning & Transformation
* Standardized date fields to isolate monthly and quarterly trend cycles.
* Deduplicated transactions and resolved null entries for customer location markers.
* Computed derived metrics: `Total Sales`, `Units Sold`, and `Revenue per Region`.

### Stage 3: Data Modeling & Analysis
* **Category Share Analysis:** Calculated exact category contribution split (Toys: 20.46%, Clothing: 19.55%, Electronics: 20.20%, Furniture: 20.07%, Books: 19.73%).
* **Regional Insights:** Multi-axis cross-tabulation comparing `Customer Count` vs. `Total Sales` across key cities (**Alexandria, Aswan, Cairo, Giza, Mansoura**).
* **Product-Level Drilldown:** Aggregated sales performance across individual product lines (e.g., Puzzles, Tablets, Laptops, Jackets, Textbooks).

### Stage 4: Dashboard Implementation & UI Design
* Built an interactive dashboard featuring executive KPI scorecards, a dynamic monthly slicer panel, and 4 primary chart visualizations:
  1. **Dual-Axis Column Chart:** Regional Customer Count vs. Total Sales Volume.
  2. **Donut Chart:** Percentage share by Product Category.
  3. **Trend Line Chart:** Monthly Sales Trajectory for 2024.
  4. **Categorized Bar Chart:** Granular revenue breakdown by item/product.

---

## 🖼️ Dashboard Preview

<img width="1386" height="603" alt="image" src="https://github.com/user-attachments/assets/6d780c41-4777-41dc-8e79-f28508cffe76" />

---

## 🛠️ Tools Used

* **Microsoft Excel / Power BI:** Data modeling, dynamic chart construction, dashboard layout, and interactive timeline slicers.
* **Pivot Tables & Calculated Measures:** Aggregation engine for KPI calculations and regional metrics.
* **Data Visualization:** Dual-axis charts, donut chart breakdown, time-series line trends, and grouped product bar charts.

---
