# Financial Statement Analysis Dashboard | German Market Case Study

## 1. Project Overview

This project analyzes the financial performance of **EuroFit Workplace Solutions GmbH**, a synthetic company operating in the German and European workplace solutions market.

The dataset covers monthly financial data from **2023 to 2025** and includes income statement, balance sheet, cash flow, budget, accounts receivable, and accounts payable data.

The dashboard focuses on financial statement analysis to help management understand whether business growth is translating into profit, cash flow, and a healthy financial position.

The reporting currency is **EUR**.

## 2. Business Problem

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

## 3. Report Audience

This dashboard is designed for the management team, especially:

- CEO / Founder
- CFO / Finance Manager
- COO
- Commercial Director

The report supports decisions related to growth, profitability, cost control, cash flow, working capital, and financial planning.

## 4. Dataset and Data Model

The dataset contains multiple financial tables used to build a management-level financial statement dashboard.

### Main Tables

| Table | Description |
|---|---|
| Dim_Date | Calendar table for monthly and yearly analysis |
| Dim_Product | Product and category information |
| Dim_Channel | Sales channel information |
| Dim_Customer | Customer, country, segment, and industry information |
| Fact_Revenue | Revenue transactions including units, price, discount, COGS, and gross profit |
| Fact_Expense | Operating expenses by department, cost group, and cost behavior |
| Fact_Balance_Sheet | Monthly balance sheet data |
| Fact_Cash_Flow | Monthly cash flow movements |
| Fact_Budget | Budget data for variance analysis |
| Fact_AR_AP | Accounts receivable and accounts payable data |

### Data Model Logic

The data model mainly follows a star-schema approach, with **Dim_Date** as the central time dimension connected to all financial fact tables.

Product, channel, customer, and country fields are used mainly for revenue and geographic analysis. Financial statement tables such as expense, balance sheet, cash flow, budget, and AR/AP are analyzed through their own reporting line fields, such as cost group, line item, cash flow line, budget line, and aging bucket.

The relationship view below shows how dimension tables connect to the main fact tables in Power BI.

![Data Model](images/Relationship.png)
