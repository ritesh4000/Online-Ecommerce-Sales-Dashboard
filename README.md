# 📊 Olist E-Commerce Sales Dashboard | Power BI

## 📑 Table of Contents

* [📌 Project Overview](#-project-overview)
* [🎯 Business Problem](#-business-problem)
* [📊 Dashboard Preview](#-dashboard-preview)
* [📈 Key KPIs](#-key-kpis)
* [📊 Dashboard Pages](#-dashboard-pages)
* [💡 Key Business Insights](#-key-business-insights)
* [🔗 Data Model](#-data-model)
* [🧹 Data Cleaning & Transformation](#-data-cleaning--transformation)
* [🧮 DAX & Calculations](#-dax--calculations)
* [🛠️ Tools & Technologies](#️-tools--technologies)
* [🎓 Skills Demonstrated](#-skills-demonstrated)
* [📁 Project Files](#-project-files)
* [🚀 Future Improvements](#-future-improvements)
* [👤 Author](#-author)

---

# 📌 Project Overview

This project presents an interactive **Olist E-Commerce Sales Dashboard** developed using **Microsoft Power BI**.

The objective of this project is to analyze e-commerce business performance and provide meaningful insights into:

* Sales performance
* Order trends
* Customer behavior
* Product and category performance
* Seller performance
* Payment methods
* Delivery performance
* Customer reviews
* Geographic performance

The dashboard allows users to interact with the data using filters and visualizations to understand business performance and identify important trends.

---

# 🎯 Business Problem

An e-commerce business generates a large amount of data from customers, orders, products, sellers, payments, and reviews.

The main challenge is to convert this raw data into meaningful business information.

This project answers questions such as:

* How are sales performing over time?
* Which product categories generate the most sales?
* Which states have the highest number of customers?
* What are the most popular payment methods?
* How long does it take to deliver orders?
* Which products and sellers perform best?
* What is the customer review performance?
* Which areas contribute the most to business performance?

---

# 📊 Dashboard Preview

## 🏠 Main Dashboard

![Main Dashboard]()<img width="1522" height="842" alt="01_Main_Dashboard png" src="https://github.com/user-attachments/assets/39edbee4-4e0c-455b-b059-9a448b2a4024" />



The main dashboard provides an executive-level overview of the business using KPIs, charts, filters, and interactive visualizations.

---

## 💰 Product Analysis

![Product Analysis]()<img width="1497" height="856" alt="02_Sales_Analysis png" src="https://github.com/user-attachments/assets/aaee0921-a163-4e17-bb6c-d75276efd8a7" />


This page focuses on:

* Sales trends
* Order trends
* Revenue performance
* Category performance
* Monthly/yearly sales
* Geographic sales performance

---

## 👥 Region Analysis

![Region Analysis]()<img width="1540" height="840" alt="03_Region_Analysis png" src="https://github.com/user-attachments/assets/79733d03-2986-43f6-a58c-5006a1b6b2aa" />



This page analyzes:

* Customer distribution
* Customer locations
* Customer purchasing behavior
* Orders by region/state
* Customer trends

---


## 🔗 Delivery analysis()<img width="1518" height="827" alt="04_Delivery_Analysis png" src="https://github.com/user-attachments/assets/fc2bfc02-98c8-41c0-9fd3-2a8e03759565" />


* Estimated Delivery Date
* Actual Delivery Date
* Delivery Delay
* On-Time Delivery
* Delayed Orders
* Delivery Performance by State
* Average Delivery Time
* Order Delivery Status


## 🔗 Data Model

![Data Model]()<img width="1437" height="817" alt="05_Data_Model png" src="https://github.com/user-attachments/assets/ee28e384-8935-4b67-91a0-d37e9de4b721" />


The Power BI data model shows relationships between important tables such as:

* Customers
* Orders
* Order Items
* Products
* Sellers
* Payments
* Reviews

A proper relational model helps create accurate and efficient analysis.

---

## 🧹 Data Cleaning & Transformation

![Data Cleaning]()<img width="1880" height="1073" alt="06_Data_Cleaning png" src="https://github.com/user-attachments/assets/7a98c9d1-934e-4a49-ac5c-842b4719458b" />


Data preparation was performed using **Power Query**.

Major steps included:

* Removing unnecessary columns
* Handling missing values
* Removing duplicate records
* Correcting data types
* Renaming columns
* Creating calculated columns
* Merging/transforming data
* Validating the dataset

---

# 📈 Key KPIs

The dashboard focuses on important business KPIs such as:

| KPI                      | Purpose                         |
| ------------------------ | ------------------------------- |
| 🛒 Total Orders          | Measures total number of orders |
| 💰 Total Sales           | Measures overall sales/revenue  |
| 👥 Total Customers       | Measures customer base          |
| 📦 Total Products        | Measures product availability   |
| ⭐ Average Review Score   | Measures customer satisfaction  |
| 🚚 Average Delivery Time | Measures delivery performance   |
| 💳 Payment Performance   | Analyzes payment methods        |

---

# 📊 Dashboard Pages

The project contains multiple analytical sections:

### 1. 🏠 Executive Dashboard

Overall business performance and KPIs.

### 2. 💰 product Analysis

Sales and order trends across time and categories.

### 3. 👥 Customer Analysis

Customer distribution and purchasing behavior.

### 4. 📦 region Analysis

Product and category performance.

### 5. 🚚 Delivery Analysis

Delivery time and operational performance.

### 6. ⭐ Review Analysis

Customer satisfaction and review scores.

---

# 💡 Key Business Insights

The dashboard can be used to identify insights such as:

### 📌 product

* Identify periods with the highest sales.
* Analyze sales trends over time.
* Identify high-performing categories.

### 📌 Customers

* Identify states with the highest customer concentration.
* Understand geographic customer distribution.
* Analyze customer purchasing patterns.

### 📌 region

* Identify top-performing product categories.
* Find products with high demand.
* Compare category-level performance.

### 📌 Delivery

* Analyze average delivery time.
* Identify areas with slower deliveries.
* Compare estimated and actual delivery performance.

### 📌 Reviews

* Analyze customer satisfaction.
* Identify categories receiving better or lower ratings.
* Understand the relationship between delivery and customer reviews.

> **Note:** Final insights should be updated according to the actual results shown in your dashboard.

---

# 🔗 Data Model

The project uses Power BI's relational data modeling capabilities.

### Main Tables

```text
Customers
    ↓
Orders
    ↓
Order Items
    ↓
Products

Orders
    ↓
Payments

Orders
    ↓
Reviews

Order Items
    ↓
Sellers
```

The relationships between these tables allow analysis across different business dimensions.

---

# 🧹 Data Cleaning & Transformation

Data preparation was performed using **Power Query**.

### Main Transformation Steps

1. Imported the dataset into Power BI.
2. Checked the structure of each table.
3. Corrected data types.
4. Removed unnecessary columns.
5. Handled missing/null values.
6. Removed duplicate records where required.
7. Renamed columns for better readability.
8. Created required calculated columns.
9. Checked relationships between tables.
10. Validated the final dataset before visualization.

---

# 🧮 DAX & Calculations

DAX was used to create business measures and calculations.

Examples of calculations include:

```DAX
Total Orders = DISTINCTCOUNT(Orders[order_id])
```

```DAX
Total Customers = DISTINCTCOUNT(Customers[customer_id])
```

```DAX
Average Review Score = AVERAGE(Reviews[review_score])
```

Additional measures were created based on the requirements of the dashboard.

---

# 🛠️ Tools & Technologies

### 📊 Power BI

Used for:

* Dashboard development
* Data visualization
* Data modeling
* Interactive reporting

### 🧹 Power Query

Used for:

* Data cleaning
* Data transformation
* Data preparation

### 🧮 DAX

Used for:

* Measures
* KPIs
* Business calculations
* Analytical metrics

### 📁 Excel / CSV

Used as data sources and for initial data inspection.

---

# 🎓 Skills Demonstrated

This project demonstrates the following Data Analyst skills:

### Data Analysis

* Data Cleaning
* Data Transformation
* Exploratory Data Analysis
* Business Analysis
* KPI Analysis

### Power BI

* Dashboard Development
* Data Modeling
* Interactive Visualizations
* Slicers & Filters
* Drill-through
* Tooltips
* Conditional Formatting
* Report Design

### DAX

* Calculated Measures
* Aggregations
* Time-based Analysis
* Business KPIs

### Data Modeling

* Relationships
* Fact & Dimension Tables
* Data Validation
* Relational Data Modeling

### Business Intelligence

* Performance Analysis
* Trend Analysis
* Customer Analysis
* Product Analysis
* Operational Analysis
* Decision Support

---

# 📁 Project Files

```text
📦 Olist-Ecommerce-Dashboard
│
├── 📄 README.md
│
├── 📊 Olist E-Commerce Dashboard.pbix
│
├── 📄 Olist Dashboard.pdf
│
├── 📁 Images
│   ├── 🖼️ 01_Main_Dashboard.png
│   ├── 🖼️ 02_Sales_Analysis.png
│   ├── 🖼️ 03_Customer_Analysis.png
│   ├── 🖼️ 04_Product_Analysis.png
│   ├── 🖼️ 05_Data_Model.png
│   └── 🖼️ 06_Data_Cleaning.png
│
├── 📁 Documentation
│   ├── 📄 Business_Problem.pdf
│   ├── 📄 Key_Insights.pdf
│   └── 📄 Data_Dictionary.pdf
│
└── 📁 Dataset
    └── Dataset files
```

---

# 🔗 Dashboard Navigation

| Section              | Link                                                      |
| -------------------- | --------------------------------------------------------- |
| 🏠 Main Dashboard    | [View Dashboard](Images/01_Main_Dashboard.png)            |
| 💰 Sales Analysis    | [View Sales Analysis](Images/02_Sales_Analysis.png)       |
| 👥 Customer Analysis | [View Customer Analysis](Images/03_Customer_Analysis.png) |
| 📦 Product Analysis  | [View Product Analysis](Images/04_Product_Analysis.png)   |
| 🔗 Data Model        | [View Data Model](Images/05_Data_Model.png)               |
| 🧹 Data Cleaning     | [View Data Cleaning](Images/06_Data_Cleaning.png)         |
| 📊 Power BI File     | [Download/View PBIX](Olist%20E-Commerce%20Dashboard.pbix) |
| 📄 Dashboard PDF     | [View Dashboard PDF](Olist%20Dashboard.pdf)               |

---

# 🚀 Future Improvements

Future versions of this project could include:

* 📈 Sales Forecasting
* 👥 Customer Segmentation
* 🎯 RFM Analysis
* 🔮 Predictive Analytics
* 📊 Profitability Analysis
* 🚚 Delivery Delay Prediction
* 🤖 Machine Learning Integration
* 📅 Advanced Time-Series Analysis

---

# ⭐ Project Highlights

### What makes this project valuable?

✔ Real-world e-commerce dataset

✔ Interactive Power BI dashboard

✔ Multiple business perspectives

✔ Data cleaning and transformation

✔ Relational data modeling

✔ DAX-based KPIs

✔ Business-focused insights

✔ Interactive filters and visualizations

✔ Portfolio-ready Data Analyst project

---

# 👤 Author

## Ritesh Rathod

**Aspiring Data Analyst**

### Skills

`SQL` • `Power BI` • `Excel` • `Power Query` • `DAX` • `Data Analysis` • `Data Visualization`

---

⭐ If you found this project useful, consider giving the repository a **Star**.
