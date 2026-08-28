# 📊 Financial Health Dashboard — Power BI

## 📌 Project Overview

The **Financial Health Dashboard** is an interactive Business Intelligence project developed using **Microsoft Power BI** as part of my **CodeAlpha Power BI Internship**.

The dashboard provides a comprehensive view of an organization's financial performance by analyzing revenue, expenses, profitability, assets, liabilities, cash flow, and future revenue trends.

It enables users to interactively analyze financial performance across different **years, departments, and regions**.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Monitor overall financial performance
- Analyze revenue and expenses
- Calculate net profit and profit margin
- Compare actual revenue with budgeted revenue
- Analyze assets and liabilities
- Monitor operating and closing cash flow
- Analyze financial trends over time
- Forecast future revenue
- Provide interactive filtering by Year, Department, and Region

---

## 📊 Dashboard Features

### KPI Cards

The dashboard contains five major financial KPIs:

- Total Revenue
- Total Expenses
- Net Profit
- Profit Margin
- Net Cash Flow

These KPIs provide a quick overview of the organization's financial health.

### Interactive Filters

Users can dynamically analyze the dashboard using:

- Year
- Department
- Region

### Financial Analysis Visuals

The dashboard includes:

- Monthly Profitability
- Net Profit Trend
- Revenue vs Budget Trend
- Assets vs Liabilities
- Net Assets Trend
- Closing Cash Trend
- Operating Cash Flow
- Revenue Trend & 6-Month Forecast

---

## 🔮 Revenue Forecasting

A **6-month revenue forecast** was implemented using Power BI's forecasting capabilities.

The forecast uses historical revenue trends to estimate future financial performance and includes a **confidence interval** to represent the possible range of future revenue values.

---

## 🧮 DAX Measures

Several DAX measures were created for financial analysis.

### Total Revenue

```DAX
Total Revenue =
CALCULATE(
    SUM(FactTransactions[Amount]),
    DimAccount[Account Type] = "Revenue"
)