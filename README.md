# 🛍️ Customer Shopping Behavior Analysis

> An end-to-end data analytics project that analyzes customer purchasing behavior, product preferences, discount usage, subscription patterns, and customer segments using **Python, MySQL, SQL, and Power BI**.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![NumPy](https://img.shields.io/badge/NumPy-Data%20Processing-blue)
![SQL](https://img.shields.io/badge/SQL-Analysis-orange)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)

---

## 📌 Project Overview

Understanding customer shopping behavior is essential for improving customer retention, optimizing marketing strategies, and increasing revenue.

This project analyzes transactional data from **3,900 customer purchases** across different product categories to identify patterns in:

- Customer spending
- Customer segments
- Product preferences
- Discount usage
- Subscription behavior
- Shipping preferences
- Purchase frequency
- Customer demographics

The project follows an end-to-end analytics workflow, starting with **data cleaning and feature engineering in Python**, followed by **SQL-based business analysis using MySQL**, and finally presenting insights through an **interactive Power BI dashboard**.

---

## 🎯 Project Objectives

The primary objectives of this project are to:

- Understand customer purchasing patterns
- Identify high-value customer segments
- Analyze subscription behavior
- Evaluate the impact of discounts on purchasing
- Identify top-performing products
- Analyze customer spending across demographics
- Understand shipping preferences
- Generate actionable business recommendations

---

## 📊 Dataset Summary

| Attribute          | Details       |
| ------------------ | ------------- |
| **Total Records**  | 3,900         |
| **Total Columns**  | 18            |
| **Missing Values** | 37            |
| **Missing Column** | Review Rating |
| **Database**       | MySQL    |
| **Dashboard**      | Power BI      |

### Dataset Features

#### 👤 Customer Demographics

- Age
- Gender
- Location
- Subscription Status

#### 🛍️ Purchase Details

- Item Purchased
- Category
- Purchase Amount
- Season
- Size
- Color

#### 📈 Shopping Behavior

- Discount Applied
- Promo Code Used
- Previous Purchases
- Frequency of Purchases
- Review Rating
- Shipping Type

---

## 🛠️ Tools & Technologies

| Technology           | Purpose                               |
| -------------------- | ------------------------------------- |
| **Python**           | Data cleaning and feature engineering |
| **Pandas**           | Data manipulation and analysis        |
| **NumPy**            | Numerical operations                  |
| **MySQL**            | Database storage and analysis         |
| **SQL**              | Business analysis                     |
| **Power BI**         | Interactive visualization             |
| **Jupyter Notebook** | Data analysis and experimentation     |

---

## 🔄 Project Workflow

```text
Raw Dataset
     │
     ▼
Data Cleaning & Preparation
     │
     ▼
Feature Engineering using Python
     │
     ▼
MySQL Database Integration
     │
     ▼
SQL-Based Business Analysis
     │
     ▼
Power BI Dashboard
     │
     ▼
Business Insights & Recommendations
```

---

## 🧹 Data Preparation

Python and Pandas were used to clean and prepare the dataset for analysis.

### Data Cleaning

The following steps were performed:

- Loaded the dataset using Pandas
- Explored the dataset using `info()` and `describe()`
- Checked for missing values
- Identified **37 missing values** in the `Review Rating` column
- Imputed missing review ratings using the **median rating of the corresponding product category**
- Renamed columns into `snake_case` format

### Feature Engineering

Additional features were created to improve the analysis:

- Created an `age_group` column by categorizing customers based on age
- Created a `purchase_frequency_days` feature from purchase frequency data
- Compared `discount_applied` and `promo_code_used` to identify redundancy
- Removed the redundant `promo_code_used` column

### Database Integration

The cleaned dataset was then:

1. Connected to MySQL using Python
2. Loaded into a MySQL database
3. Prepared for SQL-based business analysis

---

## 📈 SQL Business Analysis

MySQL was used to answer key business questions related to customer behavior and revenue.

### Questions Answered

1. How does total revenue compare between male and female customers?

2. Which customers used discounts but still spent more than the average purchase amount?

3. Which five products have the highest average review ratings?

4. How do average purchase amounts compare between Standard and Express shipping?

5. How do subscribers and non-subscribers compare in terms of average spending and total revenue?

6. Which five products have the highest percentage of discounted purchases?

7. How can customers be classified as **New, Returning, or Loyal** based on purchase history?

8. What are the top three most-purchased products in each category?

9. Are customers with more than five purchases more likely to subscribe?

10. Which age groups contribute the most revenue?

---

## 📊 Power BI Dashboard

An interactive Power BI dashboard was developed to visualize the results of the analysis.

The dashboard helps analyze:

- 👥 Customer demographics
- 💰 Revenue and purchase patterns
- ⭐ Product performance
- 🎟️ Discount usage
- 🔄 Customer segments
- 📦 Shipping preferences
- 👑 Subscription behavior
- 📈 Revenue contribution by age group

## 💡 Business Insights

The analysis is designed to provide insights into several areas of customer behavior:

### 👥 Customer Segmentation

Customers can be classified into:

- **New Customers**
- **Returning Customers**
- **Loyal Customers**

based on their purchase history.

### 💰 Customer Spending

The analysis compares customer spending across:

- Gender
- Age groups
- Subscription status
- Shipping preferences
- Discount usage

### 🎟️ Discount Behavior

Customers who use discounts are analyzed to determine whether discounts lead to higher purchase values and how heavily different products depend on promotional pricing.

### ⭐ Product Performance

Products are evaluated based on:

- Average review ratings
- Purchase frequency
- Discount usage
- Category-level performance

### 👑 Subscription Behavior

Subscriber and non-subscriber groups are compared based on:

- Average spending
- Total revenue
- Purchase frequency
- Customer purchase history

---

## 💼 Business Recommendations

Based on the analysis, the following strategies can be considered:

### 🚀 Boost Subscriptions

Promote exclusive benefits, offers, and incentives to increase subscription adoption.

### 🏆 Develop Loyalty Programs

Reward repeat customers and encourage returning customers to become loyal customers.

### 🎟️ Review Discount Policies

Analyze the relationship between discounts and purchasing behavior to balance sales growth with profitability.

### ⭐ Improve Product Positioning

Use highly rated and frequently purchased products in targeted marketing campaigns.

### 🎯 Targeted Marketing

Focus marketing campaigns on high-revenue customer segments and age groups.

### 📦 Optimize Shipping Options

Analyze customer preferences for Standard and Express shipping to improve the overall customer experience.

---

## 📂 Project Structure

```text
Customer_Behaviour_Analysis/
│
├── Python/
│   └── customer_shopping_behavior.ipynb
│
├── SQL/
│   └── business_analysis_queries.sql
│
├── PowerBI/
│   └── customer_behavior_dashboard.pbix
│
├── Screenshots/
│   └── dashboard.png
│
├── README.md
└── requirements.txt
```

> Update the structure above if the actual filenames or folders in the repository are different.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Karan-Dhingra-05/Customer_Behaviour_Analysis.git

cd Customer_Behaviour_Analysis
```

### 2. Create a Virtual Environment

#### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv venv

source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install pandas numpy jupyter psycopg2-binary
```

Or, if `requirements.txt` is available:

```bash
pip install -r requirements.txt
```

---

## 🐍 Run the Python Analysis

1. Start Jupyter Notebook:

```bash
jupyter notebook
```

2. Open the notebook inside the `Python` directory.

3. Update the dataset path if required.

4. Run the notebook cells sequentially.

The notebook performs:

```text
Data Loading
     ↓
Data Exploration
     ↓
Data Cleaning
     ↓
Missing Value Treatment
     ↓
Feature Engineering
     ↓
PostgreSQL Integration
```

---

## 🗄️ MySQL Setup

### 1. Create a MySQL Database

Create a database using MySQL.

### 2. Configure the Database Connection

Update the MySQL connection details in the Python notebook according to your local environment.

Example:

```python
import psycopg2

connection = psycopg2.connect(
    host="localhost",
    database="your_database",
    user="your_username",
    password="your_password",
    port="5432"
)
```

> Do not commit database passwords, API keys, or other credentials to GitHub.

### 3. Load the Cleaned Dataset

The cleaned DataFrame is loaded into MySQL for further SQL analysis.

---

## 🧮 Run SQL Analysis

Navigate to:

```text
SQL/business_analysis_queries.sql
```

Run the SQL queries against the MySQL database to reproduce the business analysis.

The SQL analysis covers:

- Revenue analysis
- Customer segmentation
- Product performance
- Discount analysis
- Subscription behavior
- Shipping preferences
- Age-group revenue analysis

---

## 📊 Open the Power BI Dashboard

Open the Power BI file:

```text
PowerBI/customer_behavior_dashboard.pbix
```

using **Microsoft Power BI Desktop**.

If required:

1. Update the MySQL connection.
2. Verify the data source.
3. Refresh the dataset.
4. Explore the interactive dashboard.

---

## 🎯 Skills Demonstrated

This project demonstrates practical experience in:

- Python
- Pandas
- NumPy
- Data Cleaning
- Data Preprocessing
- Feature Engineering
- Exploratory Data Analysis
- MySQL
- SQL
- Business Analytics
- Customer Segmentation
- Revenue Analysis
- Product Analytics
- Power BI
- Data Visualization
- Business Insight Generation

---

## 📌 Conclusion

This project demonstrates a complete **end-to-end data analytics workflow**.

Starting with raw transactional data, the project uses **Python and Pandas** for data cleaning and feature engineering, **MySQL and SQL** for structured business analysis, and **Power BI** for interactive visualization.

The analysis transforms customer transaction data into meaningful insights around:

- Customer spending
- Product performance
- Subscription behavior
- Discount usage
- Customer segmentation
- Shipping preferences
- Revenue contribution

The project highlights how data analytics can be used to support **customer-focused marketing, retention strategies, product positioning, and data-driven business decisions**.
