# Sales Data Analysis

## Overview
This project performs an exploratory data analysis (EDA) on a dataset containing sales data from an e-commerce platform. The objective is to derive meaningful insights and trends, such as identifying top-selling products, customer purchasing behavior, and revenue trends, and to provide actionable recommendations for business improvements.

## Objectives
- Analyze monthly revenue trends to understand peak sales periods.
- Identify products that are frequently sold together.
- Determine the most sold product and explore reasons behind its popularity.
- Analyze customer purchase patterns by time (hour, day, and month).
- Provide actionable insights for marketing and inventory optimization.

## Dataset
The dataset used for this analysis contains the following columns:
- **Order ID**: Unique identifier for each order.
- **Product**: Name of the purchased product.
- **Quantity Ordered**: Quantity of the product purchased.
- **Price Each**: Price of a single unit of the product.
- **Order Date**: Timestamp of the purchase.
- **Purchase Address**: Customer's location.

### Data Preprocessing
1. **Merging Data**: Monthly sales data files were combined into a single dataset.
2. **Data Cleaning**: Addressed missing or invalid values and corrected data types.
3. **Feature Engineering**: Added new columns, such as Month, Hour, and Sales (calculated as `Quantity Ordered` × `Price Each`).

## Analysis and Insights

### 1. Monthly Revenue Trends
- **Goal**: Identify peak sales months to plan marketing campaigns and inventory.
- **Visualization**: A bar chart was used to show revenue trends by month.
- **Insight**: December showed the highest sales, likely due to holiday shopping.

### 2. Frequently Sold Together Products
- **Goal**: Identify product combinations often bought together to optimize bundling strategies.
- **Method**: Analyzed `Order ID` to find products purchased together.
- **Insight**: Certain product combinations (e.g., phones with charging accessories) were common.

### 3. Most Sold Product
- **Goal**: Identify the product with the highest sales volume and investigate reasons for its popularity.
- **Finding**: A low-priced product (AAA batteries) was the most sold due to its affordability and necessity.

### 4. Purchase Patterns by Hour
- **Goal**: Understand the times when customers are most active.
- **Visualization**: A line chart was used to show customer activity by hour.
- **Insight**: Sales peaked around 11 AM and 7 PM, suggesting ideal times for marketing.

### 5. Customer Locations
- **Goal**: Analyze geographic trends in sales.
- **Visualization**: A bar chart was used to show sales by city.
- **Insight**: Cities like San Francisco and New York showed the highest sales.

## Recommendations
1. **Marketing Campaigns**:
   - Schedule promotional emails and advertisements during peak hours (11 AM and 7 PM).
   - Focus campaigns on December to capitalize on the holiday shopping season.
2. **Bundling Products**:
   - Offer discounts on frequently purchased product combinations.
   - Create bundles like "Phone + Charger" to increase revenue.
3. **Inventory Optimization**:
   - Stock popular products, especially high-demand items like USB-C cables, AAA batteries.
   - Increase inventory for December and other peak months.

## Tools and Technologies
- **Python Libraries**: Pandas, Matplotlib, Seaborn.
- **Visualization**: Bar charts and line graphs to present insights.
- **IDE**: Jupyter Notebook.

## How to Run the Project
1. Install the required libraries:
   ```bash
   pip install pandas matplotlib seaborn
   ```
2. Open the Jupyter Notebook `Pandas_sales_analysis.ipynb`.
3. Run the cells sequentially to execute the analysis.

## Future Enhancements
- Use machine learning models to forecast future sales.
- Build an interactive dashboard using tools like Tableau or Power BI.
- Incorporate external data, such as weather or economic indicators, for deeper insights.



