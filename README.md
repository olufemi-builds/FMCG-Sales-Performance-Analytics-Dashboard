# FMCG Sales Performance Analytics Dashboard

## Project Overview

This project analyzes FMCG sales performance using a synthetic dataset to simulate real-world retail business reporting. The analysis focuses on product performance, regional trends, customer segmentation, and profitability insights.

It demonstrates how FMCG companies track KPIs and make data-driven decisions using Power BI and structured data analysis.

---

## Business Problem

FMCG companies need to understand:
- which products drive revenue
- regional performance differences
- profit contribution by category
- customer buying patterns
- overall business performance trends

This project provides a structured dashboard approach to solve these needs.

---

## Dataset Description

The dataset contains 5,000 FMCG sales transactions with the following fields:

- order_id: Unique transaction ID  
- date: Transaction date  
- product_name: FMCG product name  
- category: Product category (Hygiene, Baby, Beauty)  
- region: Sales region  
- quantity_sold: Units sold per order  
- unit_price: Selling price per unit  
- cost_price: Cost per unit  
- revenue: Total sales value  
- profit: Total profit  
- customer_type: Retail or Wholesale  

---

## Key KPIs

- Total Revenue  
- Total Profit  
- Total Quantity Sold  
- Profit Margin  
- Average Order Value  

---

## Power BI Dashboard Structure

### Executive Summary
- Total Revenue (Card)
- Total Profit (Card)
- Total Quantity Sold (Card)
- Profit Margin (Card)
- Monthly Revenue Trend (Line Chart)

---

### Product Analysis
- Top 10 Products by Revenue (Bar Chart)
- Bottom 10 Products by Revenue
- Category performance breakdown
- Profitability comparison across products

---

### Regional Analysis
- Revenue by Region (Bar Chart or Map)
- Profit by Region
- Region performance ranking table

---

### Customer Analysis
- Retail vs Wholesale revenue comparison
- Category contribution to total sales

---

## Key Insights

### 1. Revenue Concentration
A small number of products contribute a large share of total revenue.

### 2. Regional Differences
Some regions consistently outperform others in both revenue and profit.

### 3. Category Performance
Beauty and Hygiene categories generate the highest revenue contribution.

### 4. Profitability Variation
Some high-revenue products have lower margins due to cost differences.

---

## Business Recommendations

- Focus marketing on top-performing product categories  
- Improve distribution in underperforming regions  
- Optimize pricing strategy for low-margin products  
- Strengthen wholesale performance channels  
- Align inventory with demand patterns  

---

## Tools Used

- Power BI (Dashboard creation and visualization)  
- Excel (Data handling)  
- Python (Dataset generation)  

---

## Dataset Generation

A synthetic FMCG dataset of 5,000 records was generated using Python to simulate real-world retail sales patterns including pricing, product categories, and regional distribution.

---

## DAX Measures Used

```DAX
Total Revenue = SUM(fmcg_sales_data[revenue])

Total Profit = SUM(fmcg_sales_data[profit])

Total Quantity Sold = SUM(fmcg_sales_data[quantity_sold])

Profit Margin = DIVIDE([Total Profit], [Total Revenue])

Average Order Value = DIVIDE([Total Revenue], COUNT(fmcg_sales_data[order_id]))
