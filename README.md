# Financial Statement Analysis Dashboard | German Market Case Study

## 1. Project Summary

This project analyzes the financial performance of **EuroFit Workplace Solutions GmbH**, a synthetic company operating in the German and European workplace solutions market.

The dashboard focuses on financial statement analysis, including revenue performance, profitability, cost structure, balance sheet health, cash flow, and working capital. It is designed to help management understand whether business growth is financially sustainable.

## 2. Project Context

EuroFit Workplace Solutions GmbH provides workplace-related products and services, including ergonomic office products, workplace wellness services, and digital subscriptions.

The dataset covers monthly financial data from **2023 to 2025**. It reflects a realistic financial reporting environment with income statement, balance sheet, cash flow, budget, accounts receivable, and accounts payable data.

The reporting currency is **EUR**.

## 3. Business Problem

The company is growing, but management needs to understand whether this growth creates real financial value.

The key business question is:

> Is revenue growth translating into profit, cash flow, and a healthy financial position?

To answer this question, the dashboard focuses on:

- How revenue changes over time
- Whether gross margin and operating profit are healthy
- Which cost areas put pressure on profitability
- How assets, liabilities, and equity change over time
- Whether profit is converted into operating cash flow
- Whether AR/AP and working capital create financial risk

## 4. Report Audience

This dashboard is designed for the management team, especially:

- CEO / Founder
- CFO / Finance Manager
- COO
- Commercial Director

The report supports decisions related to growth, profitability, cost control, cash flow, working capital, and financial planning.

## 5. Dataset and Data Model

The dataset contains multiple financial tables used to build a management-level financial statement dashboard.

### Main Tables

| Table | Description |
|---|---|
| Dim_Date | Calendar table for monthly and yearly analysis |
| Dim_Product | Product and category information |
| Dim_Channel | Sales channel information |
| Dim_Customer | Customer, country, segment, and industry information |
| Dim_Account | Financial account structure |
| Fact_Revenue | Revenue transactions including units, price, discount, COGS, and gross profit |
| Fact_Expense | Operating expenses by department, cost group, and cost behavior |
| Fact_Balance_Sheet | Monthly balance sheet data |
| Fact_Cash_Flow | Monthly cash flow movements |
| Fact_Budget | Budget data for variance analysis |
| Fact_AR_AP | Accounts receivable and accounts payable data |

### Data Model Logic

The model follows a star-schema approach. Fact tables store revenue, expenses, balance sheet values, cash flow movements, budget data, and AR/AP records. Dimension tables provide context for time, product, customer, channel, and account analysis.

Key relationships include:

| Relationship | Purpose |
|---|---|
| Dim_Date → Fact_Revenue | Analyze revenue by month and year |
| Dim_Date → Fact_Expense | Analyze expenses over time |
| Dim_Date → Fact_Balance_Sheet | Track financial position by period |
| Dim_Date → Fact_Cash_Flow | Analyze cash flow movements |
| Dim_Date → Fact_Budget | Compare actual results with budget |
| Dim_Date → Fact_AR_AP | Analyze AR/AP aging and payment timing |
| Dim_Product → Fact_Revenue | Analyze revenue and margin by product |
| Dim_Channel → Fact_Revenue | Compare sales performance by channel |
| Dim_Customer → Fact_Revenue | Analyze performance by customer, country, and segment |
| Dim_Account → Fact_Balance_Sheet | Support balance sheet reporting structure |
| Dim_Account → Fact_Cash_Flow | Support cash flow reporting structure |
