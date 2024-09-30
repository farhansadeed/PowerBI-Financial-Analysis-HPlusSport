# PowerBI-Financial-Analysis-HPlusSport
An interactive Power BI dashboard analyzing H+ Sport's financial performance to identify profit drivers, product profitability, and regional variations. This project supports Landon Hotel Management's decision-making process for potential acquisition by providing actionable insights into sales, costs, and profits.

# :man_student:Dashboard::electron:

![DashBoard.png](https://github.com/farhansadeed/PowerBI-Financial-Analysis-HPlusSport/blob/main/DashBoard.png)

## Dataset

The dataset includes monthly aggregated financial data from 2012 to 2014, covering:

- **Date**: Monthly dates, aggregated with the day always being the first.
- **Units Sold**: Number of units sold per product.
- **Sales Price**: Selling price per unit.
- **Manufacturing Price**: Cost to produce each unit (COGS).
- **Gross Sales**: Calculated as Units Sold × Sales Price.
- **COGS**: Calculated as Units Sold × Manufacturing Price.
- **Discounts**: Any discounts applied to sales.
- **Profit**: Calculated using the relationship Sales = COGS + Profit.

Financial Relationships Used:
- **Sales** = COGS + Profit
- **Gross Sales** = Sales + Discounts
- **Units Sold × Sales Price** = Gross Sales
- **Units Sold × Manufacturing Price** = COGS

## Analyses Performed

1. COGS and Profit Over Time:

- **Challenge**: Initial visualization displayed overlapping data for January across years.
- **Solution**: Adjusted the X-axis to use 'Date' instead of 'Date Hierarchy' for correct time-series representation.
- **Visualization**: Used a stacked column chart to represent discrete monthly data effectively.

2. Financial Data Formatting:

- **Issue**: Y-axis labels were in millions and not displaying financial figures appropriately.
- **Solution**: Changed the data type of financial columns (Gross Sales, Discounts, Sales, COGS, Profit) to 'Currency' for proper financial representation.
#Enhancements:
- **Removed unnecessary axis titles.
- **Enabled total labels with one decimal place for clarity.
- **Positioned the legend at the bottom center.

3. Product Profitability Analysis:

- **Improvement**: Replaced standard slicers with a tree map to provide a visual representation of product profitability.
- **Visualization**: The tree map displays products categorized by profit, enhancing engagement and insight.

Date Slicer Synchronization:
- **Problem**: Date slicer was incorrectly showing data from 2022 to 2024.
- **Solution**: Implemented a relative date slicer with an anchor date to ensure consistency and correct data range from 2012 to 2014.

4. Key Performance Indicators (KPIs):

- Last Month's Sales:
- Created a measure to calculate sales from the most recent month.
- Average Profit Over Time:
- Calculated the average profit across the entire data period.
- Last Month's Profit:
- Developed a measure to display profit figures for the last month of data.
- Display: Positioned KPIs prominently on the dashboard for quick reference.

5.Geographical Analysis:

- Objective: Identify profit variations and losses across different countries.
- Method: Used maps and charts to visualize regional performance.
- Outcome: Highlighted countries with higher profits and those incurring losses to guide strategic decisions.

6. Profit Drivers Identification:

- Approach: Analyzed various factors such as product categories, regions, and time periods to determine what drives profit.
- Visualization: Employed interactive charts to drill down into specific areas influencing profitability.

## Tools Used:

- **Microsoft Power BI**: For data modeling, analysis, and creating interactive dashboards.
- **Data Visualization Techniques**:
**Stacked Column Charts
**Tree Maps
**Slicers and Filters
**Interactive KPIs
- **Data Preparation**:
**Data cleansing and formatting.
**Correcting date hierarchies and financial data types.
**Implementing measures and calculations for KPIs.
