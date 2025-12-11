# 🛒 Customer Shopping Behavior Analysis
A complete end-to-end data analytics project using **Python**, **SQL**, and **Power BI** to understand and improve customer purchasing behavior.

---

## 📌 1. Project Overview

This project analyzes **3,900 retail transactions** to understand shopping patterns across demographics, product categories, seasons, and purchase channels.  
The goal is to uncover how factors like **discounts**, **reviews**, **shipping type**, and **subscription status** influence customer decisions — helping businesses improve **sales**, **satisfaction**, and **loyalty**.

---

## 📂 2. Dataset Summary

- **Total Rows:** 3,900  
- **Columns:** 18  
- **Key Features:**
  - Demographics: `age`, `gender`, `location`, `subscription_status`
  - Purchase Details: `item_purchased`, `category`, `purchase_amount`, `season`, `size`, `color`
  - Behavioral Data: `discount_applied`, `previous_purchases`, `review_rating`, `shipping_type`
- **Missing Data:** 37 missing values in `review_rating`

---

## 🧹 3. Data Cleaning & EDA (Python)

All initial data preparation was performed using Python.

### ✔ Steps Performed:
- **Loaded & Inspected Data**
  - Used `pandas` (`.info()`, `.describe()`)
- **Handled Missing Values**
  - Imputed missing `review_rating` using **median per product category**
- **Standardized Column Names**
  - Converted all column names to `snake_case`
- **Feature Engineering**
  - Created `age_group` (binned age categories)
  - Derived `purchase_frequency_days`
  - Dropped redundant column: `promo_code_used`
- **Database Integration**
  - Loaded cleaned data into **PostgreSQL** for SQL-based analysis

---

## 🗄️ 4. SQL Analysis (Business Insights)

SQL queries were used to extract key business insights.

### 🔍 Key Questions Solved:
1. **Revenue by Gender**
2. **High-Spending Customers Using Discounts**
3. **Top 5 Highest Rated Products**
4. **Standard vs. Express Shipping Comparison**
5. **Subscribers vs. Non-Subscribers Revenue Comparison**
6. **Most Discount-Dependent Products**
7. **Customer Segmentation:** New, Returning, Loyal
8. **Top 3 Purchased Products per Category**
9. **Are heavy purchasers more likely to subscribe?**
10. **Revenue Distribution by Age Group**

---

## 📊 5. Power BI Dashboard

An interactive Power BI dashboard was created to visualize:

- Sales by Gender, Category, Age Group  
- Rating-based product performance  
- Discount impact analysis  
- Subscription-based customer value  
- Shipping preference patterns  
- Customer segmentation (New, Returning, Loyal)

The dashboard enables filtering, comparison, and deep insights for decision-makers.

---

## 🎯 6. Business Recommendations

Based on SQL and dashboard insights:

### ✔ Increase Subscriptions  
Provide exclusive benefits to encourage sign-ups.

### ✔ Strengthen Customer Loyalty  
Introduce tier-based rewards to convert returning customers to loyal ones.

### ✔ Optimize Discount Strategy  
Balance discount usage to avoid margin loss.

### ✔ Improve Product Positioning  
Promote top-rated and frequently purchased items.

### ✔ Target High-Value Segments  
Focus on:
- Revenue-leading age groups  
- Express-shipping users  
- Loyal customers  

---

## 🛠️ 7. Tech Stack

| Area | Tools |
|------|-------|
| **Data Cleaning & EDA** | Python (Pandas, NumPy) |
| **Database** | PostgreSQL / MS SQL Server |
| **Visualization** | Power BI |
| **Environment** | Jupyter Notebook, SSMS |

---

## 📁 8. Recommended Folder Structure
```bash
Customer-Shopping-Behavior-Analysis/
│
├── raw_dataset.csv
│
├── eda_and_cleaning.ipynb
│
├── business_queries.sql
│
├── powerbi_dashboard.pbix
│
├── Presentaion.pptx
│
├── KK Report Customer Shopping Behavior Analysis.pdf
│
└── README.md
```

--- 

## 🚀 9. How to Run This Project

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/customer-shopping-behavior-analysis.git
```

### 2️⃣ Install Python Dependencies
```bash
pip install -r requirements.txt
```
### 3️⃣ Run the Jupyter Notebook
```bash
jupyter notebook notebooks/eda_and_cleaning.ipynb
```
### 4️⃣ Execute SQL Scripts
Run all SQL queries in:
```bash
sql/business_queries.sql
```
### 5️⃣ Open Power BI Dashboard

Open:
```
dasahboard/powerbi_dashboard.pbix
```
## 🙌 Conclusion

This project uses Python, SQL, and Power BI to analyze customer shopping behavior and deliver insights on spending patterns, demographics, product preferences, and loyalty indicators.

---
