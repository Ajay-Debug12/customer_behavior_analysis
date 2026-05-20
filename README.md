# 🛒 E-Commerce Customer Behavior Analysis

An end-to-end Exploratory Data Analysis (EDA) project using Python to analyze customer purchasing behavior, identify revenue drivers, and generate actionable business insights from real-world e-commerce transaction data.

---

## 📌 Project Objective

The goal of this project is to answer key business questions such as:

- Who are the most valuable customers?
- Which products generate the highest revenue?
- Which countries contribute the most sales?
- What are the monthly, weekly, and hourly sales trends?
- How is customer spending distributed?
- What business recommendations can improve revenue and retention?

---

## 📂 Dataset

This project uses the **Online Retail II** dataset from the UCI Machine Learning Repository, available on Kaggle.

🔗 Dataset Link: https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci

### Dataset Features

- Invoice
- StockCode
- Description
- Quantity
- InvoiceDate
- Price
- Customer ID
- Country

### Dataset Size

- 1M+ transaction records
- Multiple countries
- Real-world retail data from 2009–2011

---

## 🛠️ Tools & Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Git & GitHub

---

## 📊 Project Workflow

### 1. Data Loading
- Imported the dataset into Google Colab.

### 2. Data Understanding
- Checked shape, columns, data types, and descriptive statistics.

### 3. Data Cleaning
- Removed duplicate rows.
- Removed missing `Customer ID`.
- Removed cancelled invoices.
- Removed invalid quantities and prices.
- Converted `InvoiceDate` to datetime.

### 4. Feature Engineering
Created new columns:
- Revenue = Quantity × Price
- Year
- Month
- MonthNumber
- DayOfWeek
- Hour

### 5. Exploratory Data Analysis
Performed analysis on:
- Revenue trends
- Top products
- Top countries
- Top customers
- Customer spending distribution
- Correlation analysis

### 6. Business Insights & Recommendations
Summarized key findings and strategic recommendations.

---

## 📈 Key Performance Indicators (KPIs)

- Total Revenue
- Total Orders
- Total Customers
- Average Order Value (AOV)

---

## 📉 Visualizations Created

- Monthly Revenue Trend
- Revenue by Day of Week
- Revenue by Hour
- Top 10 Products by Revenue
- Top 10 Countries by Revenue
- Customer Spending Distribution (Log Scale)
- Correlation Heatmap

---

## 🔍 Key Insights

- A small percentage of customers contributes a significant portion of total revenue.
- Revenue peaks during specific months, indicating seasonal buying patterns.
- A few products generate the majority of revenue.
- The United Kingdom contributes the highest share of sales.
- Customer spending is highly right-skewed, with a handful of high-value customers.

---

## 💡 Business Recommendations

- Launch loyalty programs for top-spending customers.
- Increase marketing before peak months.
- Focus on promoting high-performing products.
- Investigate countries with low sales for growth opportunities.
- Reduce returns by reviewing problematic products.

---

## 📁 Project Structure

```text
ecommerce-customer-behavior-analysis/
│── data/
│   └── online_retail_II.csv
│
│── notebooks/
│   └── Ecommerce_Customer_Behavior_Analysis.ipynb
│
│── visuals/
│   ├── monthly_revenue_trend.png
│   ├── top_products.png
│   ├── top_countries.png
│   ├── customer_spending_distribution.png
│   └── correlation_heatmap.png
│
│── cleaned_data/
│   └── cleaned_ecommerce_data.csv
│
│── README.md
