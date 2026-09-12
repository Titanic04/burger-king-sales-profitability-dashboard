# 🍔 Burger King Sales & Profitability Dashboard

A Power BI portfolio project focused on analyzing restaurant sales, store performance, product profitability, order channels, peak hours, and potential root causes of low profitability.

> **Disclaimer:** This is a portfolio/learning project created using synthetic Burger King-style data. It is not official Burger King corporate data and is not affiliated with Burger King or Restaurant Brands Asia.

---

## 📊 Project Overview

The objective of this project is to transform raw restaurant sales data into meaningful business insights using Microsoft Power BI.

Instead of focusing only on revenue, the dashboard follows a business-analysis approach:

**What is happening? → Where is the problem? → What could be causing it? → What business action can be taken?**

The dashboard provides an interactive view of sales performance, store performance, profitability, products, order channels, peak hours, and geographic performance.

---

## 🎯 Business Objectives

- Analyze overall sales and revenue performance
- Identify high-performing products and categories
- Compare store revenue and profitability
- Identify stores with lower profit margins
- Analyze peak ordering hours
- Compare profitability across order channels
- Analyze geographic revenue performance
- Investigate potential root causes of low profitability
- Support data-driven business decisions

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **DAX**
- **Power Query / Data Preparation**
- **Microsoft Excel**
- **Data Modeling**
- **Data Visualization**

---

## 🗂️ Dataset

The project uses a synthetic Burger King-style restaurant dataset created for portfolio and learning purposes.

### Dataset includes:

| Table | Records | Purpose |
|---|---:|---|
| Orders | 5,000 | Main transaction/fact table |
| Customers | 1,200 | Customer information |
| Products | 25 | Product and category information |
| Stores | 15 | Store and geographic information |
| Calendar | 546 | Date dimension |
| Read_Me | - | Dataset documentation |

### Analysis Period

**01 January 2025 – 30 June 2026**

---

## 🧩 Data Model

The project follows a **Star Schema**.

### Fact Table
- Orders

### Dimension Tables
- Customers
- Products
- Stores
- Calendar

### Relationships

```text
Customers
    │
    │ Customer_ID
    ▼
  Orders
    ▲
    │ Product_ID
Products

Stores
    │
    │ Store_ID
    ▼
  Orders

Calendar
    │
    │ Date
    ▼
  Orders
