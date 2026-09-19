#E-Commerce Sales Data Analysis

Data Analytics | Business Analytics | Exploratory Data Analysis | Sales Analytics | Customer Analytics | Data Cleaning | Data Visualization

A Python-based Data Analytics and E-Commerce Sales Analysis project that cleans, explores, analyzes, and visualizes transactional sales data to identify revenue trends, customer patterns, product-category performance, high-value orders, returns, and relationships between numerical variables.

Data Analytics Focus

This project demonstrates an end-to-end data analytics workflow for converting raw transactional data into actionable business insights. It covers data quality assessment, data cleaning, exploratory data analysis (EDA), KPI analysis, customer and product analytics, revenue analysis, return analysis, and data visualization.

Recruiter-relevant keywords: Data Analytics, Data Analysis, Business Analytics, Exploratory Data Analysis (EDA), Data Cleaning, Data Wrangling, Data Transformation, KPI Analysis, Sales Analytics, Customer Analytics, Revenue Analysis, Data Visualization, Business Insights, Python, Pandas, NumPy, Matplotlib, Seaborn.

Project Overview

This project uses Pandas, NumPy, Matplotlib, and Seaborn to perform an end-to-end exploratory data analysis (EDA) workflow on an e-commerce sales dataset.

The analysis covers:

Data inspection and profiling

Missing-value handling

Date and datatype conversion

Revenue and sales KPIs

Category and regional analysis

Customer demographic analysis

High-value order identification

Returned-order analysis

Correlation analysis

Data visualization

Export of a cleaned dataset

Dataset

The dataset contains 1,000 e-commerce transactions and 12 columns.

Dataset Columns

Column

Description

Customer ID

Unique customer identifier

Gender

Customer gender

Region

Customer/order region

Age

Customer age

Product Name

Purchased product

Category

Product category

Unit Price

Price per unit

Quantity

Number of units purchased

Total Price

Total transaction value

Shipping Fee

Shipping charge

Shipping Status

Current shipping/order status

Order Date

Transaction date

Categories

Electronics

Accessories

Wearables

Products

Laptop

Smartphone

Monitor

Keyboard

Mouse

Headphones

Smartwatch

Key Dataset Statistics

Based on the supplied dataset:

Transactions: 1,000

Total revenue: $1,346,600

Average order value: $1,346.60

Total items sold: 3,008

Median customer age: 49 years

Electronics transactions: 477

Accessories transactions: 401

Wearables transactions: 122

Data Cleaning

The project identifies and handles missing values in:

Age

Region

Shipping Status

Cleaning steps include:

Convert Order Date to a datetime datatype.

Fill missing Age values using the median age.

Fill missing Region values with Unknown.

Fill missing Shipping Status values with Unknown.

Export the cleaned dataset as a new CSV file.

The original dataset contains:

100 missing Age values

50 missing Region values

50 missing Shipping Status values

The cleaning workflow is implemented in E_Commerce.py.

Analysis Performed

1. Sales KPIs

The project calculates:

Total Revenue

Average Order Value

Total Items Sold

Average Customer Age

2. Revenue by Product Category

Revenue is aggregated by Category and sorted in descending order to identify the categories contributing the most revenue.

3. Orders by Region

The project counts transactions across:

West

South

East

North

Unknown

4. Customer Demographics

Customers are grouped into age segments:

18–25

26–35

36–45

46–55

56+

Revenue is then compared across age groups and genders.

5. High-Value Orders

Orders with:

Total Price > $1,000

are identified and their total contribution to revenue is calculated.

6. Returned Orders

The project identifies orders where:

Shipping Status == "Returned"

and calculates:

Number of returned orders

Revenue associated with returned orders

Number of returned laptop orders

7. Correlation Analysis

A correlation matrix is generated for:

Age

Unit Price

Quantity

Total Price

Shipping Fee

A heatmap is used to visualize potential relationships between numerical variables.

Visualizations

The Python script generates visualizations including:

Monthly revenue trend

Revenue by product category

Correlation heatmap

The visualizations are created using Matplotlib and Seaborn.

Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter / VS Code

Project Structure

E-Commerce-Sales-Analysis/
│
├── E_Commerce.py
├── Ecommerce_Sales.csv
├── cleaned_e_commerce_sales_data.csv
└── README.md
