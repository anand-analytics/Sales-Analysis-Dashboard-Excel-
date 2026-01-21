
# ☕ Coffee Sales Analysis Dashboard (Excel)

## 📌 Project Overview
This project is an end-to-end **Microsoft Excel dashboard** designed to analyze coffee sales performance across products, customers, and countries. It demonstrates how raw transactional data can be transformed into an **interactive, insight-driven dashboard** using Excel’s advanced formulas, pivot tables, and visualization tools.

The dashboard enables users to explore sales trends over time, compare performance by coffee type and geography, and identify top customers through dynamic filtering.

---

## 🎯 Objectives
- Analyze coffee sales trends over time  
- Compare sales performance by coffee type and country  
- Identify top-performing customers  
- Enable interactive, user-driven analysis without manual recalculation  

---

## ✨ Key Features
- **Dynamic Visualizations**
  - Line chart showing total sales trends by coffee type
  - Bar charts for sales by country and top customers

- **Interactive Filtering**
  - Timeline for time-based analysis
  - Slicers for roast type, package size, and loyalty card status

- **Automated Data Gathering**
  - Dynamic lookups across multiple tables using Excel formulas
  - Automatic refresh of pivot tables when data is updated

- **Clean UI/UX**
  - Gridlines and headers removed
  - Dashboard styled as a standalone analytical application

---

## 🗂️ Data Structure
The Excel workbook is organized into three primary tables:

1. **Orders**
   - Order ID
   - Order Date
   - Customer ID
   - Product ID
   - Quantity

2. **Customers**
   - Customer Name
   - Email
   - Country
   - Loyalty Card Status

3. **Products**
   - Coffee Type
   - Roast Type
   - Package Size
   - Unit Price
   - Profit Margin

---

## 🔧 Technical Implementation

### 1️⃣ Data Gathering & Transformation
- **XLOOKUP**
  - Retrieved customer details (name, email, country) from the Customers table

- **INDEX MATCH**
  - Used as a flexible alternative for product-related lookups across multiple columns

- **Nested IF Logic**
  - Handled missing data (e.g., blank emails)
  - Converted abbreviations into readable values (e.g., *Rob* → *Robusta*)

- **Calculated Columns**
  - Created a `Sales` field by multiplying unit price with quantity sold

---

### 2️⃣ Data Cleaning & Formatting
- Applied custom date formats (`DD-MMM-YYYY`) for clarity
- Added unit labels (kg) to package sizes
- Standardized all monetary values in **USD**
- Converted data ranges into **Excel Tables** for automatic pivot refresh
- Performed duplicate checks to ensure data integrity

---

### 3️⃣ Data Analysis & Visualization
- Built multiple **Pivot Tables** for aggregation by:
  - Month
  - Country
  - Customer

- **Line Chart**
  - Displays sales trends for Arabica, Excelsa, Liberica, and Robusta

- **Bar Charts**
  - Sales by Country (USA, Ireland, UK)
  - Top 5 Customers by Sales

- **Slicers & Timeline**
  - Connected across all visuals using *Report Connections*
  - Enables synchronized filtering across the entire dashboard

---

## ▶️ How to Use
1. Open `Coffee_Sales_Dashboard.xlsx`
2. Use the **Timeline** to select months or years
3. Apply **Slicers** to filter by:
   - Roast Type
   - Package Size
   - Loyalty Card Status
4. Add new data to the Orders table and refresh pivot tables to update the dashboard

---

## 🛠️ Tools Used
- Microsoft Excel
  - Pivot Tables & Pivot Charts
  - XLOOKUP
  - INDEX MATCH
  - Nested IF statements
  - Slicers & Timeline
![Dashboard Preview](https://github.com/anand-analytics/Sales-Analysis-Dashboard-Excel-/blob/main/Sales%20Dashboard.png)

