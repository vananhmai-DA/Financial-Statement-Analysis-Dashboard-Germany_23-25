# Data-warehouse-project-Python-SQL-POWER-BI
## 1. Project Context

VietDist Corporation is a distribution company that manages sales transactions, sales targets, customer information, product master data, employee data, distributor records, return transactions, and promotion programs across multiple file-based sources such as Google Drive and OneDrive.

Currently, the company’s data is stored in different file formats, including CSV, XLSX, XLSM, and XLSB. This creates challenges in data consolidation, data quality control, and timely business reporting.

This project aims to build an end-to-end Sales Performance and Distribution Analytics Platform. The data pipeline ingests raw files from cloud storage, loads them into PostgreSQL, transforms them through the Bronze, Silver, and Gold layers, and provides analytical data marts for Power BI reporting.

## 2. Business Problem

VietDist needs a centralized analytics platform to monitor sales performance, compare actual sales against targets, evaluate employee and distributor performance, analyze product and regional performance, and track return transactions.

Without a structured data pipeline and analytical data model, business users may rely on scattered spreadsheets, manual reporting, and inconsistent calculations. This can lead to delayed insights, data quality issues, and less effective decision-making.

## 3. Project Objective

The objective of this project is to design and build a complete local analytics pipeline that connects to Google Drive and OneDrive data sources, loads raw data into PostgreSQL, cleans and standardizes data in the Silver layer, builds analytical star schema and mart tables in the Gold layer, and supports interactive Power BI dashboards for sales and distribution analysis.
