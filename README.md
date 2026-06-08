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

The dataset is a synthetic financial dataset covering monthly data from **2023 to 2025**. It includes revenue, expenses, balance sheet, cash flow, budget, and AR/AP data.

The data model mainly uses **Dim_Date** as the central time dimension. Product, channel, and customer fields support revenue analysis, while financial statement tables are analyzed through their own reporting line fields such as cost group, line item, cash flow line, budget line, and aging bucket.

The relationship view below shows the final Power BI data model.

![Data Model](images/Relationship.png)
