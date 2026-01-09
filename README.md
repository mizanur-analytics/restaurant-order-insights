# Project Background
Restaurants generate massive amounts of order data, but without analysis, this data does not guide decision-making.  
This project analyzes three months of international restaurant order data to identify:
- What customers buy the most and least  
- Which cuisines and categories drive revenue  
- How customer order size impacts sales  
The goal is to help restaurant managers improve menu design, pricing, and promotions using data.
![My_SQL_Restaurant_Projects_1](https://github.com/user-attachments/assets/610962b0-42ca-437e-b240-c88b092b3ef3)
# Restaurant Order Analysis
**Project Type:** SQL Data Analytics + Business Intelligence  
**Dataset:** Restaurant Orders (Quarterly Transaction Data)  
**Tools:** MySQL / PostgreSQL, Excel, Power BI / Tableau  
# Data Structure
The dataset contains two tables: <a href = "https://github.com/mizanur-analytics/restaurant-order-insights/blob/main/create_restaurant_db.sql">restaurant_db</a>
## `menu_items`
| Column        | Description                               |
|---------------|-------------------------------------------|
| menu_item_id  | Unique ID for each menu item              |
| item_name     | Name of the dish                          |
| category      | Cuisine or food type (Italian, Asian, etc.) |
| price         | Price of the item                         |

## `order_details`
| Column            | Description               |
|-------------------|---------------------------|
| order_details_id  | Line-level ID             |
| order_id          | Unique order number       |
| order_date        | Date of order             |
| item_id           | Menu item purchased       |
Each row in `order_details` represents one item in an order.
# Business Questions Answered
## Menu Performance
- How many items are on the menu?
- What are the cheapest and most expensive items?
- How many Italian dishes exist and what are their price ranges?
- Which categories have the most items and highest average prices?
## Order Behavior
- What is the date range of the data?
- How many total orders and items were sold?
- Which orders had the most items?
- How many large orders (12+ items) occurred?
## Revenue Analysis
- Which menu items and categories are most and least ordered?
- Which orders generated the highest revenue?
- What did the highest-spending customers buy?
# Process
1. Loaded both tables into SQL  
2. Profiled menu data (price, category, item count)  
3. Analyzed order volume and order sizes  
4. Joined `order_details` with `menu_items`  
5. Calculated item popularity and revenue per order  
6. Built a dashboard for business users  
# Executive Summary
## Overview of Findings
- A small number of menu items drive most sales  
- Some categories have many items but low demand  
- Large group orders generate a significant share of revenue  
## Sales Trends
- Orders cluster around specific dates and meal periods  
- High-value orders tend to include premium-priced items  
## Product Performance
- Certain dishes sell frequently but are underpriced  
- Some expensive dishes sell rarely and reduce menu efficiency  
![My_SQL_Restaurant_Projects_3](https://github.com/user-attachments/assets/693246d2-dd09-4207-83d5-109863b749f5)
# Project Insights
## Quantified Value
- Top 20% of items generate nearly 60% of total orders  
- Large orders (12+ items) contribute disproportionately to revenue  
## Business Metrics Impact
- Identifies which items should be promoted  
- Flags low-selling, low-profit dishes for removal  
- Helps optimize pricing by category  
## Simple Story
The restaurant does not have a demand problem — it has a **menu focus problem**.  
A few items are doing most of the work, while many items add complexity without adding profit.
# Final Conclusions & Recommendations
## For Restaurant Management
- Promote high-selling, high-margin dishes  
- Remove or reprice low-selling menu items  
- Bundle popular items into combo deals  
## For Marketing Teams
- Focus ads on best-selling cuisines  
- Target promotions to large-group orders  
## For Operations
- Stock ingredients based on top-selling items  
- Reduce waste by eliminating low-demand dishes  
