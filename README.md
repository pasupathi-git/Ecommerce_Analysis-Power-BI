# Ecommerce Analysis – Power BI

## 🔍 Project Overview

This project presents an in-depth analysis of 50,000+ transactions from the Brazilian E-Commerce Public Dataset (Olist). The objective was to move beyond standard reporting and uncover key revenue drivers, cost inefficiencies, and profitability risks impacting overall performance.

---

## 📈 Key Analytical Insights

• Revenue Concentration: The top 10 product categories account for 60% of total revenue, indicating high dependency on limited segments.

• Scale of Operations: Evaluated $13.59M in total revenue across multi-category transactions.

• Profitability Flagging: Developed a custom Freight Ratio metric to identify SKUs where shipping costs exceeded product value, flagging potential loss-makers.

• Data Refinement: Performed structured data cleaning, column standardization, and dashboard optimization for professional clarity and usability.

---

## 💡 Business Impact

• Enables strategic prioritization of high-performing product categories  
• Identifies unprofitable SKUs due to logistics cost imbalance  
• Supports data-driven pricing and freight optimization decisions  
• Improves operational visibility into revenue and cost structure  

---

## 📂 Visualizations

### 1. Revenue Distribution by Product Category
![Revenue Distribution](Visualizations/Revenue%20Distribution%20by%20Product%20Category.png)

### 2. Freight Cost vs Total Revenue
![Freight Cost](Visualizations/Freight%20Cost%20vs.%20Total%20Revenue.png)

### 3. Freight Ratio by Product ID
![Freight Ratio](Visualizations/Total%20Revenue%20and%20Freight%20Ratio%20by%20product_ID.png)

---

### 🧮 Key DAX Formulas
To drive these insights, I engineered custom measures using DAX best practices:

* **Total Revenue:** `Total Revenue = SUM(Order_Items[price])`
* **Freight Ratio (Profitability Metric):** `Freight Ratio = DIVIDE(SUM(Order_Items[freight_value]), [Total Revenue])`
* **Top 10 Category Revenue:** Used `TOPN` logic to identify that 10 categories drive 60% of the $13.59M total.

---

## 🛠️ Technical Highlights

Data Source: Brazilian E-Commerce Public Dataset (Kaggle – Olist)

Tool: Power BI

Key Files:

• Ecommerce_Analysis.pbix – Complete data model and dashboard  
• DataSet/ – Raw transaction data  
• Visualizations/ – Exported dashboard views  

