# 📊 Retail Sales Analysis & Interactive Dashboard (2024)

An interactive retail performance dashboard designed to track high-level sales metrics, analyze regional customer distributions, evaluate category trends, and monitor item-level revenue streams for 2024.
---

## 🚀 Project Overview

This repository documents the full lifecycle of building a retail analytics solution—from raw data extraction to dynamic data visualization. The dashboard tracks key business KPIs including revenue growth, unit sales volume, top-performing SKUs, and regional performance across five major product categories and key Egyptian metropolitan cities.
<img width="1386" height="603" alt="image" src="https://github.com/user-attachments/assets/6d780c41-4777-41dc-8e79-f28508cffe76" />
---

## 📌 Executive Summary KPI Cards

* **Total Sales:** $6,977,094.80
* **Units Sold:** 90,294
* **Top Selling Product:** Doll ($522,606)
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

## 💡 Key Business Insights

1. **Overall Performance:** Generated **$6,977,094.80** in total sales with **90,294 units sold**. The **Doll Product** was the top-selling item, bringing in **$522,606**.
2. **Category Balance:** Revenue is evenly split across all categories: **Toys** leads at **20.46%**, followed by **Furniture** (20.20%), **Electronics** (20.07%), **Books** (19.73%), and **Clothing** (19.55%).
3. **Monthly Trends:** Sales trajectory peaks in **April** (exceeding $7.3M), followed by a steady run through mid-year and a dip around February ($6.8M range).
4. **Geographic Distribution:** Active customer count remains evenly balanced (56 to 62 customers per city), with **Aswan** and **Mansoura** demonstrating top sales volume relative to customer numbers.
5. **Product Performers:** Top category drivers include **Dolls, Puzzles, and Shirts**, while sub-items like **Sofas** and **Headphones** generated lower overall revenue.
---

## 📊 Dashboard Key Components & Visuals

### 1. Interactive Slicers & Dynamic Controls
* **Region Slicer:** Filter dynamic metrics by key regional markets (**Alexandria**, **Aswan**, **Cairo**, **Giza**, **Mansoura**).
* **Date Timeline / Filter:** Granular monthly filtering capability across 2024 data (May–Dec focus shown).

### 2. Customer Count vs. Total Sales by Region
* **Visual Type:** Dual-Axis Combo Chart (Bar & Column).
* **Metrics Tracked:** `Count of CustomerID` against `Total Sales in Millions`.
* **Regions Analyzed:** Alexandria, Aswan, Cairo, Giza, Mansoura.

### 3. Category Breakdown (All Categories Ordered)
* **Visual Type:** Donut Chart.
* **Distribution Percentage:**
  * **Clothing:** 20.46%
  * **Electronics:** 20.20%
  * **Furniture:** 20.07%
  * **Toys:** 19.73%
  * **Books:** 19.55%

### 4. Trend of Sales for 2024
* **Visual Type:** Line Chart (Sales Trajectory over Time).
* **Metrics:** Total sales per month in millions ($6.5M – $7.4M range).
* **Key Observations:** Highlights revenue fluctuations, peaking around April 2024 before stabilizing in late Q3/Q4.

### 5. Product-Level Breakdown (Sales per Product)
* **Visual Type:** Clustered Column Chart grouped by Product Category.
* **Product Taxonomy:**
  * **Toys:** Puzzle, Lego, Doll, Car Toy, Ball
  * **Furniture:** Wardrobe, Table, Sofa, Chair, Bed
  * **Electronics:** Tablet, Phone, Laptop, Headphones, Camera
  * **Clothing:** Shoes, Shirt, Pants, Jacket, Dress
  * **Books:** Textbook, Novel, Notebook, Magazine, Comics
---

## 🛠️ Project Stages & Workflow
<img width="790" height="100" alt="image" src="https://github.com/user-attachments/assets/5cf9b537-a053-447e-a317-125486d1b3f6" />

### Stage 1: Data Collection & Intake
* Gathered transactional records for 2024 containing dates, regions, customer IDs, product sub-categories, sales revenue, and quantities sold.
* Schema mapping across 5 core product categories: **Toys, Furniture, Electronics, Clothing, and Books**.

### Stage 2: Data Cleaning & Transformation
* **Power Query / Data Cleaning:** Pre-processed transaction logs (handled blank values, standardized region names, dynamic date parsing).
* Standardized date fields to isolate monthly and quarterly trend cycles.
* Deduplicated transactions and resolved null entries for customer location markers.
* Computed derived metrics: `Total Sales`, `Units Sold`, and `Revenue per Region`.

### Stage 3: Data Modeling & Analysis
* **Power Pivot / Data Modeling:** Calculated measures for metrics using DAX/Pivot tables:
  * `Total Sales = SUM(Sales[Amount])`
  * `Units Sold = SUM(Sales[Quantity])`
  * `Customer Count = DISTINCTCOUNT(Sales[CustomerID])`
* **Custom Number Formatting:** Standardized dynamic currency formats ($ millions formatted via custom masks like `$#,##0.0,,"M"`).
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

## 🛠️ Tools Used

* **Microsoft Excel / Power BI:** Data modeling, dynamic chart construction, dashboard layout, and interactive timeline slicers.
* **Pivot Tables & Calculated Measures:** Aggregation engine for KPI calculations and regional metrics.
* **Data Visualization:** Dual-axis charts, donut chart breakdown, time-series line trends, and grouped product bar charts.

