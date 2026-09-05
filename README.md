# 🏦 Banking Analytics — End-to-End Data Analytics Project

An end-to-end banking analytics project covering data cleaning, SQL analysis, Python EDA, Microsoft Fabric data engineering, and Power BI reporting.

## 📌 Project Overview

This project analyzes banking data across customers, accounts, cards, transactions, loans, merchants, and branches.

The project follows a complete analytics workflow:

Excel → SQL → Python → Microsoft Fabric → Power BI

The goal is to transform raw banking data into meaningful business insights and an interactive analytical report.

---

## 🏗️ End-to-End Architecture

Raw Banking Data
        │
        ▼
Excel
Cleaning & Preparation
        │
        ▼
SQL
Data Analysis & Business Queries
        │
        ▼
Python
EDA & Visualization
        │
        ▼
Microsoft Fabric
Bronze → Silver → Gold
        │
        ▼
Direct Lake Semantic Model
        │
        ▼
Power BI Report

---

## 📂 Dataset

The project contains 7 main datasets:

- Customers
- Accounts
- Cards
- Loans
- Transactions
- Merchants
- Branches

---

## 🧹 1. Excel — Data Cleaning

Excel was used for initial data inspection and preparation.

Activities included:

- Reviewing source datasets
- Identifying data-quality issues
- Checking missing values
- Reviewing column types
- Preparing data for analytical processing

---

## 🗄️ 2. SQL — Banking Analytics

SQL was used to answer business questions and perform analytical exploration.

Areas analyzed:

- Customer analysis
- Account analysis
- Transaction analysis
- Loan analysis
- Aggregations
- Filtering and grouping
- Joins
- Business metrics

SQL helped validate the data and identify useful analytical patterns before building the reporting solution.

---

## 🐍 3. Python — Exploratory Data Analysis

Python was used for exploratory data analysis and visualization.

### Tools

- Python
- Pandas
- Matplotlib

### Analysis

- Dataset exploration
- Data-quality checks
- Descriptive statistics
- Distribution analysis
- Trend analysis
- Business-focused visualizations

---

## ☁️ 4. Microsoft Fabric

Microsoft Fabric was used to build the analytical data platform.

### Lakehouse Architecture

Bronze → Silver → Gold

### Bronze

Raw banking tables:

- bronze_customers
- bronze_accounts
- bronze_cards
- bronze_loans
- bronze_transactions
- bronze_merchants
- bronze_branches

### Silver

Cleaned and transformed analytical tables.

### Gold

Business-ready dimensional model:

#### Dimensions

- dim_customer
- dim_account
- dim_card
- dim_merchant
- dim_branch
- dim_date

#### Facts

- fact_transaction
- fact_loan

PySpark was used for the transformation process.

---

## ⭐ 5. Semantic Model

A Microsoft Fabric Direct Lake semantic model was created on top of the Gold layer.

The model contains:

- Dimensions
- Fact tables
- Relationships
- Business measures
- Date analysis

The semantic model acts as the analytical layer between Fabric data and Power BI.

---

## 📊 6. Power BI Report

The final Power BI solution contains 5 report pages.

### Executive Overview

High-level banking KPIs and trends.

### Customer Analytics

Customer distribution and credit-score analysis.

### Accounts & Cards

Account balances, account types, and transaction activity.

### Transaction Analytics

Transaction volume, transaction values, top accounts, and transaction details.

### Loan Analytics

Loan portfolio, interest rates, yearly loan amounts, and customers with the highest number of loans.

---

## 📐 DAX Measures

Key measures include:

- Total Customers
- Total Accounts
- Total Transactions
- Total Transaction Amount
- Average Transaction Amount
- Total Account Balance
- Average Account Balance
- Total Loan Amount
- Total Loans
- Average Interest Rate
- High Credit Score Customers

---

## 📈 Key Metrics

| Metric | Value |
|---|---:|
| Customers | 50K |
| Accounts | 75K |
| Transactions | 1M |
| Transaction Amount | $5.00bn |
| Loan Amount | $4.50bn |
| Loans | 30K |
| Average Credit Score | 574.49 |
| Average Interest Rate | 8.51 |

---

## 🛠️ Technologies

- Excel
- SQL
- Python
- Pandas
- Matplotlib
- PySpark
- Microsoft Fabric
- Fabric Lakehouse
- Delta Lake
- Direct Lake
- Semantic Models
- Power BI
- DAX
- GitHub

---

## 🎯 Business Objectives

The project aims to:

- Analyze customer demographics
- Understand account distribution
- Analyze account balances
- Evaluate transaction activity
- Identify high-value accounts
- Analyze credit scores
- Understand loan portfolio trends
- Analyze interest rates
- Identify customers with multiple loans
- Build an executive-level banking analytics report

---

## 🔄 Project Workflow

1. Collect banking datasets
2. Clean and inspect data in Excel
3. Perform analytical queries using SQL
4. Conduct EDA using Python
5. Load data into Microsoft Fabric
6. Build Bronze layer
7. Transform data into Silver
8. Build Gold dimensional model
9. Create Direct Lake semantic model
10. Create DAX measures
11. Build 5-page Power BI report
12. Publish the report to Microsoft Fabric

---

## 📁 Repository Structure

```text
banking-analytics-microsoft-fabric/
│
├── README.md
│
├── Excel/
│   └── data_cleaning/
│
├── SQL/
│   └── banking_analysis.sql
│
├── Python/
│   └── banking_eda.ipynb
│
├── Fabric/
│   ├── notebooks/
│   └── architecture/
│
├── PowerBI/
│   ├── report/
│   └── screenshots/
│
└── Documentation/
    └── project_documentation.md
