# 📊 Power BI Sales Dashboard

## 📌 Objective
The goal of this project was to create an **interactive sales dashboard** for business stakeholders to monitor **Sales, Profit, Growth trends**, and key business metrics, enabling data-driven decision-making.

---

## 📂 Dataset
- **Source:** [Superstore Sales Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
- **File Used:** `superstore_cleaned.csv` (cleaned and processed in Power BI)
- **Data Cleaning Steps:**
  - Converted date columns (`Order Date`, `Ship Date`) to **Date** format
  - Converted `Sales` & `Profit` to **Decimal Number** type
  - Removed duplicate rows
  - Renamed columns for consistent naming (underscores instead of spaces)

---

## 🛠 Tools & Skills Used
- **Power BI Desktop** – Dashboard design & visualization
- **Power Query** – Data cleaning & transformation
- **DAX** – KPI calculations (Total Sales, Total Profit, Profit Margin %, Sales Growth %)
- **Data Visualization Principles** – Clean layout, interactive filters, consistent color scheme

---

## 📊 Dashboard Features
- **KPIs:** Total Sales, Total Profit, Profit Margin %, Total Orders, Sales Growth %
- **Time-Series Analysis:** Sales trend by month/year
- **Category Analysis:** Profit by category
- **Geographical View:** Sales by region (map visual)
- **Customer Analysis:** Top 10 customers by sales
- **Interactivity:** Slicers for Category, Region, and Order Date

---

## 📈 Insights from the Dashboard
- Technology and Office Supplies are top revenue contributors
- California and New York regions lead in total sales
- Positive year-over-year sales growth
- Some categories show declining profit margins — improvement potential in discount strategies

---

## 📷 Screenshots
*(Add your Power BI dashboard screenshots here)*

---

## 📑 How to Use
1. Open `superstore_cleaned.csv` in **Power BI Desktop**
2. Load and review data model
3. Create KPIs using the following DAX measures:
   ```DAX
   Total Sales = SUM('Superstore'[Sales])
   Total Profit = SUM('Superstore'[Profit])
   Profit Margin % = DIVIDE([Total Profit],[Total Sales],0)
   Total Orders = DISTINCTCOUNT('Superstore'[Order_ID])
