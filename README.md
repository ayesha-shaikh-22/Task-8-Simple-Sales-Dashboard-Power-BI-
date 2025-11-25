
## **Project Title:**

**Superstore Sales Dashboard — Task 8 (Data Analyst Internship)**

---

##  **Dataset Used:**

`superstore_sales.csv`
(Columns: Order Date, Region, Category, Sales, Profit)

---

## **Objective:**

To design a **clean and interactive Power BI dashboard** that highlights key sales insights using visuals such as line charts, bar charts, donut charts, KPIs, and slicers.

---

## **Tools Used:**

* **Power BI Desktop** (Dashboard Creation)
* **Power Query** (Data Cleaning & Transformation)
* **DAX Measures** (KPIs)

---

## **Data Cleaning Steps (Power Query):**

1. Converted **order_date** to proper Date format.
2. Created **MonthStart** column for sorting (Date.StartOfMonth).
3. Created **MonthYear** column for readable axis labels.
4. Trimmed text fields (Region, Category).
5. Removed duplicates and checked for missing values.

---

## **Dashboard Visuals Included:**

### **KPI Cards**

* Total Sales
* Total Profit
* Profit Margin %
* Avg Sales per Order 

### **Charts**

* **Line Chart** → Sales Trend by Month
* **Bar Chart** → Sales by Region
* **Donut Chart** → Sales by Category

### **Slicers**

* Region
* Category
* MonthStart (Date filter)

---

## **DAX Measures Used:**

```dax
Total Sales = SUM('superstore_sales'[Sales])

Total Profit = SUM('superstore_sales'[Profit])

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

Total Orders = DISTINCTCOUNT('superstore_sales'[Order ID])

Avg Sales per Order = DIVIDE([Total Sales], [Total Orders], 0)
```

---

## **Key Insights:**

1. **Technology** category generated the highest overall sales contribution.
2. Sales showed a **declining trend** across the months in the dataset.
3. Some regions consistently outperform others in total sales volume.
4. Profit margin remained moderate at around **12%** overall.

---

## **How to Reproduce This Dashboard:**

1. Open **Power BI Desktop**
2. Import `superstore_sales.csv`
3. Create `MonthStart` and `MonthYear` in Power Query
4. Add DAX measures in Report View
5. Build visuals following the layout in the PDF
6. Apply slicers and formatting
7. Export Dashboard as PDF

---

## **Outcome:**

A professional, interactive sales dashboard analyzing monthly trends, regional performance, category contribution, and key KPIs — suitable for stakeholders and interview discussions.

---
