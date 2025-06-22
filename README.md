# Customer-Churn
This repository contains a customer churn analysis project using Power BI, focusing on predicting churn rates and analyzing the factors contributing to customer attrition.
# Customer Churn Analysis Dashboard

This Power BI dashboard provides a detailed analysis of customer churn behavior using demographic, service usage, and revenue data. The goal is to understand churn patterns and predict customer status using a machine learning model.

---

## 📁 Project Overview

- **Tool Used:** Power BI
- **Language:** Python (for data preprocessing)
- **Data Size:** 6,418 customer records

---

## 📊 Dashboard Features

- Age-wise and tenure-wise churn trends
- Churn rate visualized using line and stacked column charts
- Total customers, new customers, and churned customers
- Filtering by age groups and tenure groups

---

## 🧮 DAX Measures Used

```dax
Churn Rate = measures_customer[Total_churn] / measures_customer[Total Customers]

New Customers = 
CALCULATE(
    COUNTROWS(customer_data),
    customer_data[Customer_Status] = "joined"
) + 0

Total Customers = 
COUNTROWS(customer_data) + 0

Total Churn = 
CALCULATE(
    COUNTROWS(customer_data),
    customer_data[Customer_Status] = "churned"
) + 0

```

## 📊 Dashboard

![DashBoard](https://github.com/user-attachments/assets/c9381e3e-e9b0-4cd3-a30f-1351d1ed1e11)

