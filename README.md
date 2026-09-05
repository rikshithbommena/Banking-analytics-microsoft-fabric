# 🏦 Banking Analytics — End-to-End Data Analytics Project

An end-to-end banking analytics project covering data cleaning, SQL analysis, Python EDA, Microsoft Fabric data engineering, Direct Lake semantic modeling, and Power BI reporting.

The project analyzes banking data across customers, accounts, cards, transactions, loans, merchants, and branches.

## 📊 Power BI Report Preview

![Executive Overview](screenshots/Executive_Overview.png)

The Power BI report provides an interactive view of key banking metrics and business insights.

---

## Project Architecture

![Banking Analytics Architecture](architecture%20diagram.png)

## 🎯 Project Objectives

- Analyze customer demographics and credit scores
- Analyze account balances and account types
- Analyze transaction activity and transaction amounts
- Analyze loan amounts and interest rates
- Build a scalable data architecture using Microsoft Fabric
- Create a business-ready semantic model
- Develop an interactive Power BI report

---

## 🔄 End-to-End Workflow

```text
Raw Banking Data
       ↓
Excel
       ↓
Data Cleaning
       ↓
SQL Server
       ↓
SQL Analysis
       ↓
Python
       ↓
Exploratory Data Analysis
       ↓
Microsoft Fabric

## ☁️ Microsoft Fabric

The project uses Microsoft Fabric to build a modern end-to-end analytics architecture.

### Lakehouse

- **Bronze Layer** — Raw banking data
- **Silver Layer** — Cleaned and transformed data
- **Gold Layer** — Business-ready dimensional model

### Data Engineering

- PySpark transformations
- Delta tables
- Data quality validation
- Star schema design
- Dimension and fact tables

### Semantic Modeling

A Direct Lake semantic model was created on top of the Gold layer to support efficient analytical reporting.

### Power BI

The semantic model is connected to Power BI Desktop using a live connection to build the final multi-page banking analytics report.
       ↓
Bronze → Silver → Gold
       ↓
Direct Lake Semantic Model
       ↓
Power BI
       ↓
Interactive Banking Analytics Report
