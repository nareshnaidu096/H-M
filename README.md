# H-M
H&M Retail Dashboard
PHASE 1: Project Setup

✅ Step 1: Define Objectives

* Goal: Provide retail insights into sales, inventory, and customer behavior for H\&M.
* Outcomes: Enable data-driven decisions for stock management, store performance, and promotional planning.

✅ Step 2: Prepare Your Dataset

* Use: [✅ Downloaded Excel File](sandbox:/mnt/data/HM_Retail_Realistic_Dataset.xlsx)
* Clean data if needed (handle nulls, data types) using Excel or Python.
* Columns:

  * Date, Store, Product\_Category, SKU, Units\_Sold, Revenue, Inventory\_Level, Stockouts, Customer\_Visits

---

🧮 PHASE 2: Data Preparation in Tableau

✅ Step 3: Load Data into Tableau

* Open Tableau → Connect to Excel → Load your dataset
* Set correct data types (Date, String, Integer)
* Create data hierarchy (Store → SKU, Product\_Category)

✅ Step 4: Create Calculated Fields

Create the following fields in Tableau:

```text
Sell-Through Rate = SUM([Units_Sold]) / (SUM([Units_Sold]) + SUM([Inventory_Level]))
Conversion Rate = SUM([Units_Sold]) / SUM([Customer_Visits])
Inventory Turnover = SUM([Units_Sold]) / AVG([Inventory_Level])
Revenue per Visit = SUM([Revenue]) / SUM([Customer_Visits])
Stockout Rate = SUM([Stockouts]) / COUNT([Date])
```

---

📊 PHASE 3: Dashboard Development

✅ Step 5: Build KPI Tiles

Create 4–6 key performance indicators:

* Total Revenue
* Units Sold
* Conversion Rate
* Sell-Through Rate
* Inventory Turnover
* Stockout Rate

✅ Step 6: Build Visual Panels

📌 Sales Panel:

* Line Chart: Revenue over time
* Bar Chart: Revenue by Product Category
* Heatmap: Revenue by Store & Category

📌 Inventory Panel:

* Dual-axis Bar/Line: Inventory vs Units Sold
* Stockout Trend over time
* Inventory Turnover by Category

📌 Customer Panel:

* Scatter Plot: Revenue vs Customer Visits by Store
* Bubble Chart: Conversion Rate by Category

📌 Geo Panel:

* Filled Map: Revenue by Store with tooltips (Units Sold, Conversion Rate)

---

🧰 PHASE 4: Dashboard Enhancement

✅ Step 7: Add Filters and Interactivity

* Global Filters: Date, Store, Product Category
* Actions: Click on bar chart → filter other visuals

✅ Step 8: Format & Style

* Use H\&M brand colors (red, black, white tones)
* Add meaningful titles, tooltips, and axis labels
* Ensure mobile/tablet view is optimized

---

📈 PHASE 5: Review & Publish

✅ Step 9: QA & Testing

* Validate KPIs against raw Excel data
* Check for filter interactions
* Test calculated fields for accuracy
✅ Step 10: Export & Share

* Save as `.twbx` Tableau packaged workbook
* Export sample dashboard as PDF/Image
* Optionally publish to Tableau Public

---

🖥️ PHASE 6: Presentation & Documentation

✅ Step 11: Create PowerPoint Summary

Include:

* Project goal
* Key visuals
* KPIs and business insights
* Impact & value delivered

