# E-Commerce Analytics SQL Queries

This repository contains a collection of SQL queries designed to analyze e-commerce performance data. The main objective is to extract insights on session volume, order trends, conversion rates, product performance, and channel efficiency over time.

The data analyzed is derived from website session and order tables, providing valuable insights into key metrics such as revenue, session-to-order conversion rates, and cross-sell performance.

## Queries Overview

### 1.Volume Growth
This query retrieves the overall session and order volume, trended by quarter, for the entire history of the business. Special logic is applied to handle the most recent quarter due to incomplete data.

### 2.Efficiency Improvements
Shows quarterly figures for session-to-order conversion rate, revenue per order, and revenue per session since the launch of the platform.

### 3.Channel Performance
Analyzes orders from various marketing channels, including:
- Google Search (non-brand)
- Bing Search (non-brand)
- Brand Search
- Organic Search
- Direct Type-In

### 4.Session-to-Order Conversion by Channel
Displays session-to-order conversion rates for the same marketing channels by quarter, with annotations regarding periods of major optimizations.

### 5.Product Sales Trends
Provides monthly trending data for revenue, margin, and total sales by product. It also highlights seasonal patterns.

### 6.Impact of New Products
Tracks the monthly sessions to the `/products` page and calculates how the percentage of those sessions that click through to other pages has changed over time. It also computes the conversion rate from viewing a product to placing an order.

### 7.Cross-Sell Performance
After introducing a new product as a primary item, this query analyzes how well products cross-sell to one another. It tracks sales data and calculates cross-sell rates for each product.

## Setup

This project assumes you have access to an SQL database containing the following tables:
- `website_sessions`
- `orders`
- `order_items`
- `website_pageviews`

