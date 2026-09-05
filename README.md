# 🏦 Banking Analytics — Microsoft Fabric

An end-to-end banking analytics project built using **Microsoft Fabric, PySpark, SQL, Direct Lake, and Power BI**.

The project transforms raw banking data into a business-ready analytics solution using a **Bronze → Silver → Gold architecture**, a dimensional star schema, a Direct Lake semantic model, and a 5-page Power BI report.

---

## 🎯 Project Overview

The objective of this project is to analyze banking operations across:

- Customers
- Accounts
- Cards
- Transactions
- Loans
- Merchants
- Branches

The solution provides insights into customer behavior, account balances, transaction activity, credit scores, card usage, and loan portfolios.

---

## 🏗️ Architecture

```text
Raw Banking Data
       │
       ▼
┌──────────────┐
│    Bronze    │
│ Raw Tables   │
└──────────────┘
       │
       ▼
┌──────────────┐
│    Silver    │
│ Cleaned Data │
└──────────────┘
       │
       ▼
┌────────────────────┐
│       Gold         │
│ Dimensional Model  │
└────────────────────┘
       │
       ▼
┌────────────────────┐
│ Direct Lake        │
│ Semantic Model     │
└────────────────────┘
       │
       ▼
┌────────────────────┐
│    Power BI        │
│      Report        │
└────────────────────┘
