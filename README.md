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

## 5. Design Thinking Process

The dashboard was designed using a Design Thinking approach to clarify the target users, business pain points, key decision metrics, and dashboard direction before building visuals in Power BI.

![Empathize](images/Empathize.png)

![Empathy Map](images/Empathy%20Map.png)

![North Star Metric and Define POV](images/Northstar%20Metric%20%26%20Define%20POV.png)

## 6. Financial Dashboard

The dashboard is structured from high-level financial overview to detailed analysis of profitability, revenue growth, cost structure, balance sheet health, cash flow, and AR/AP risk.

### 6.1 Executive Overview

![Executive Overview](images/Overview.png)

The company shows positive financial growth, with total revenue reaching **€7.60M** and net profit reaching **€1.04M**. Net margin improved in 2025, showing that revenue growth is being converted into profit more effectively. Operating cash flow remained positive, but overdue AR reached **€761.3K**, equal to **10.03% of revenue**, creating a working capital risk. Therefore, management should continue supporting growth, but avoid expanding too aggressively until collection performance improves.

### 6.2 P&L Analysis

![P&L Analysis](images/P%26L%20Analysis.png)

Profitability improved mainly because the company controlled costs better than planned. Revenue was slightly above budget by **1.1%**, while COGS was **8.5% lower than budget** and OPEX was **8.3% lower than budget**. As a result, EBITDA reached **€1.70M**, exceeding budget by **58.7%**, with an EBITDA margin of **22.36%**. However, COGS and OPEX still absorb a large share of revenue, so management should protect gross margin and review major cost groups such as Payroll and Sales & Marketing.

### 6.3 Revenue Growth Drivers

![Revenue Growth Drivers](images/Revenue%20Growth%20Drivers.png)

Revenue growth is positive, with a **16.24% CAGR** from 2023 to 2025 and a gross profit margin of **56.72%**. Growth is mainly driven by **Germany**, which generated **€5.1M**, and by **Hardware**, which contributed **€5.9M**. Direct Sales is the largest channel, contributing **€2.7M**. However, discount increased to **8.36%**, which suggests that part of the growth may depend on stronger discounting. Management should continue investing in the main growth drivers, but monitor margin quality by market, product, and channel.

### 6.4 Cost Optimization

![Cost Optimization](images/Cost%20Optimization.png)

OPEX increased in absolute value, but cost efficiency improved because OPEX represented **34.36% of revenue**. However, **89.24% of OPEX** is classified as reviewable cost, meaning there is still room for optimization. Payroll and Sales & Marketing together account for more than **66% of total OPEX**, so these areas should be the main focus of review. The goal should not be broad cost cutting, but productivity-based optimization through payroll productivity, sales ROI, customer acquisition cost, and channel efficiency.

### 6.5 Financial Health and Balance Sheet

![Financial Health and Balance Sheet](images/Financial%20Health%20%26%20Balance%20Sheet.png)

The company’s financial position is strong and becoming healthier over time. Total assets increased from **€1.49M in 2023** to **€2.19M in 2025**, while equity grew to **€1.69M**. Liquidity is very comfortable, with current assets of **€1.40M** compared with current liabilities of only **€0.09M**, resulting in a current ratio of **15.73**. Debt-to-equity decreased to **0.30**, showing low financial leverage. The key decision is how to use the strong cash position efficiently without weakening the company’s low-risk balance sheet.

### 6.6 Cash Flow and Working Capital

![Cash Flow and Working Capital](images/Cash%20Flow%20%26%20Working%20Capital.png)

The company generates positive cash flow from its core business, but profit is not fully converted into cash. In 2025, operating cash flow increased to **€421.3K**, while net income was **€469.4K**, resulting in a cash conversion rate of **88.57%**. Working capital impact remained negative and reached **-€104.4K** in 2025, suggesting that receivables, inventory, or other working capital items are absorbing cash as the company grows. Management should improve cash collection and working capital discipline instead of focusing only on profit growth.

### 6.7 AR/AP and Cash Risk

![AR/AP and Cash Risk](images/AR%20AP%20%26%20Cash%20Risk.png)

Receivables are the main working capital risk, while payables remain limited. Open AR is **€87.08K**, but overdue AR reached **€761.43K**, equal to **10.03% of total revenue**. Some overdue receivables are concentrated in high-risk customers such as Berlin Creative Hub and Saxony Startup Studio. Since open AP exposure is small, management should focus more on AR collection than AP management. The priority is to escalate high-risk overdue customers, hold further credit orders where necessary, and tighten payment terms for customers with repeated delays.

## 7. Executive Summary

EuroFit Workplace Solutions GmbH is growing profitably and has a strong financial position, but the company should focus on improving the quality and sustainability of growth before expanding aggressively.

Total revenue reached **€7.60M**, while net profit reached **€1.04M** and net margin improved to **13.64%**. EBITDA performance is also strong, mainly supported by cost control, with EBITDA exceeding budget by **58.67%**.

Revenue growth is mainly driven by **Germany**, **Hardware**, and **Direct Sales**, which shows clear growth engines for the business. However, growth is concentrated in a few markets and product categories. Discount pressure is increasing, and overdue AR accounts for **10.03% of revenue**.

This means the business is profitable, but part of its revenue is not being converted into cash on time. Therefore, the key management priority should be **controlled growth**: continue investing in high-performing segments, protect gross margin, improve collection discipline, and optimize reviewable costs instead of simply pushing more revenue.

## 8. Business Recommendations

The recommended strategy is **controlled and profitable growth**.

Management should continue investing in **Germany**, **Hardware**, and **Direct Sales** because these are the strongest revenue drivers. However, expansion should be linked to margin quality and cash collection performance.

The company should avoid using discount as the main growth tool and introduce a clear discount approval policy to protect gross margin.

On the cost side, the focus should be productivity-based optimization rather than broad cost cutting, especially for **Payroll** and **Sales & Marketing**.

The most urgent risk is overdue AR. The company should implement a risk-based collection policy, hold further credit orders for high-risk overdue customers, and tighten payment terms for customers with repeated delays.

Since the balance sheet and cash position are strong, the company has room to grow. However, cash should only be deployed into expansion after confirming that growth can be converted into profit and cash sustainably.
