# Blinkit Dashboard

### Dashboard Link :https://btude-my.sharepoint.com/:u:/g/personal/asthamad_b-tu_de/Ea4NqCIrttJCjk3G1EqQ09ABa2F3S3VJ9fujOcZmNtaI-A?e=Zh5U1w

Here is the README file for your Blinkit Dashboard in the requested format with the same symbols:

## Problem Statement

This dashboard helps Blinkit understand its outlet performance better. It allows Blinkit to track total sales, average sales, and the number of items sold across various outlet locations, sizes, and types. Additionally, the dashboard shows item categories and sales distribution based on fat content, giving insight into the types of products sold and customer preferences. These insights help Blinkit optimize its inventory, improve its services, and identify the most profitable outlets.

### Steps followed 

- **Step 1** : Load data into Power BI Desktop, dataset is a xlsx file.
- **Step 2** : Open Power Query Editor & in the View tab under Data preview section, check "Column Distribution", "Column Quality" & "Column Profile" options.
- **Step 3** : Since by default, profiling will be opened only for 1000 rows, you need to select "Column profiling based on entire dataset".
- **Step 4** : It was observed that in none of the columns errors & empty values were present.
- **Step 5** : In the report view, under the View tab, a suitable theme was selected to align with the Blinkit brand colors.
- **Step 6** : Added visuals to represent important metrics:
  - Total Sales
  - Average Sales
  - Number of Items
  - Average Ratings
  
- **Step 7** : Created slicers for "Outlet Location Type", "Outlet Size", and "Item Type" for easy filtering of data across multiple categories.
- **Step 8** : Visuals like card, pie chart, bar chart, and line chart were added to represent sales performance by various outlet types, item categories, and outlet sizes.
  
- **Step 9** : Created a pie chart to visualize the "Fat Content" in items, categorized as "Low Fat" and "Regular".
  
- **Step 10** : A bar chart was added to show the item types and their corresponding sales numbers.
  
- **Step 11** : A line chart was used to track "Outlet Establishment" over the years, representing sales trends for different outlet sizes.
  
- **Step 12** : Calculated a new measure using DAX for the total sales by outlet size:

      Total Sales by Outlet = SUM(Blinkit_Data[Sales])
  
- **Step 13** : Created a donut chart visual to represent the "Outlet Size" distribution by sales, categorized as "Medium," "Small," and "High."
  
- **Step 14** : Added a stacked bar chart to represent "Outlet Location" distribution of total sales by Tier 1, Tier 2, and Tier 3 cities.
  
- **Step 15** : Created new measures to find average sales and number of items sold per outlet:

      Avg Sales by Outlet = AVERAGE(Blinkit_Data[Sales])
      No. of Items by Outlet = COUNT(Blinkit_Data[Item])

- **Step 16** : Published the dashboard to Power BI Service for easy access and sharing.

# Snapshot of Dashboard (Power BI Service)

![snapshot](https://github.com/madhviasthana/Blinkit_Dashboard_Sales_Analysis/blob/e3ef23b4626296b74a59b021b5e44e5624e9ac44/snapshot%20dashboard.png)

# Insights

A single-page report was created on Power BI Desktop & was then published to Power BI Service. The following inferences can be drawn from the dashboard:

### [1] Outlet Performance
   - **Total Sales**: $1.20M across all outlets.
   - **Average Sales**: $141 per outlet.
   - **Number of Items**: 8523 items sold in total.

### [2] Outlet Size
   - **High-Performing Outlets**: Medium outlets contributed the highest sales at $507.90K, followed by Small outlets with $444.79K.

### [3] Outlet Location
   - **Top Locations**: Tier 3 cities contributed the highest sales at $472.13K, followed by Tier 2 with $393.15K.

### [4] Item Categories
   - **Top-Selling Item Types**: Fruits had the highest number of items sold at 1232, followed by Snacks at 1200.

### [5] Fat Content
   - **Low Fat vs Regular**: Regular fat items were more popular, with 9K items sold compared to 3K low-fat items.

This dashboard provides Blinkit with a comprehensive overview of sales performance, helping them identify high-performing outlets, understand customer preferences in item types, and analyze trends in sales growth across different outlet sizes and locations.

