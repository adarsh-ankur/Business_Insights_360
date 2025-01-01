# Business_Insights_360

## Project Overview

AtliQ Hardware has experienced rapid growth in recent years, expanding its operations globally and serving customers through three primary **channels—retailers, direct sales, and distributors**. However, the company recently faced a major setback when a new store in America, launched based on intuition and limited Excel analysis, resulted in unforeseen losses. Meanwhile, competitors with strong analytics teams were making data-driven decisions, leaving AtliQ with no choice but to embrace a data analytics culture to remain competitive.

This project marks AtliQ’s first step into Power BI, to empower stakeholders to make better decisions using real-time analytics. The focus areas for this project span finance, sales, marketing, and supply chain operations.

I worked on this project while following the Codebasics Power BI Course, which provided me with the foundational knowledge and tools to build this end-to-end solution. Here’s a detailed breakdown of my journey:

## 📌 Project Kickoff: Key Questions to Ask Before Starting
Before diving into the project, I focused on clarifying the objectives and understanding stakeholder expectations. These were some key questions that helped guide the process:

1. What is the primary objective of building this Power BI dashboard?
2. How will the success of this project be measured?
3. What is the timeline for the project, and are there any preview milestones?
4. What hopes and fears do stakeholders have regarding this dashboard?
5. Who will be using the dashboard, and for what purpose?
6. What resources and data are required to build the dashboard?
7. Are there any specific design preferences or expectations from stakeholders?

This initial phase was critical to ensure alignment with business needs and to avoid rework later in the process.

## 📊 Understanding the Dataset

Once the project goals were clear, I explored the data the data engineering team provided. Here's a high-level view of the datasets:

### Dimension Tables

- **dim_customer:** Includes static details like customer names, markets, and platforms (e.g., Brick & Mortar, E-commerce).
- **dim_market:** Contains information on 27 distinct markets, 7 sub-zones, and 4 regions (APAC, EU, LATAM, and NAN).
- **dim_product:** Lists product categories and divisions, such as PCs, peripherals, and networking equipment.

### Fact Tables

- **fact_forecast_monthly:** Holds forecasted customer demand for improved inventory planning and cost optimization.
- **fact_sales_monthly:** Similar to the forecast table, but includes actual sold quantities.

### Additional Tables

- **freight_cost:** Transportation costs for each market.
- **gross_price:** Product pricing details.
- **pre_invoice_deductions & post_invoice_deductions:** Deductions applied before and after invoicing.
- **manufacturing_cost:** Product manufacturing costs by year.

The data engineering team ensured that the datasets were denormalized for analytics purposes. However, understanding the structure of dimension and fact tables was crucial for effective data modeling in Power BI.

## 📐 Data Modeling

Data modeling forms the foundation of any successful Power BI project. For this report, I followed the **snowflake schema** to ensure optimized performance and ease of use. Poor data modeling can negatively impact report performance, so I paid special attention to relationships, cardinality, and ensuring clean joins.

Key practices followed:

- Avoiding circular dependencies.
- Using surrogate keys for relationships.
- Creating a date table using M language for consistent time-based analysis.

![Mapping](https://github.com/user-attachments/assets/f33f824b-a3d4-40e5-93ea-8e8348dd905c)


## 📊 Dashboard Design

The dashboard was designed to address all stakeholder needs, with views tailored for **finance, sales, marketing, supply chain, and executive-level** insights. Here’s a breakdown of the key components:

### Home View

A landing page with buttons for navigation to different views:

- Info Page
- Finance View
- Sales View
- Marketing View
- Supply Chain View
- Executive View

<img width="1000" alt="Home Page" src="https://github.com/user-attachments/assets/f2f12210-45e6-44e7-ba3b-dc9f855b2079" />

### Finance View
Focused on metrics like net sales, gross margin, and profitability trends, helping stakeholders track financial performance over time.

### Sales View
Provided insights into top-performing products and customer segmentation.

### Marketing View
Included actionable data on campaign performance and strategies to boost gross margins and profitability.

### Supply Chain View
Analyzed demand forecasts, inventory management, and logistics costs for improved operational efficiency.

### Executive View
A high-level summary of the company’s overall performance, including revenue trends, market share, and key metrics for decision-making.

## 🔧 Techniques & Tools Used

This project required me to master several Power BI features and techniques, including:

- DAX Language: Creating calculated columns and measures.
- Bookmarks & Page Navigation: Switching seamlessly between visuals.
- Dynamic Titles: Updating visual titles based on applied filters.
- Conditional Formatting: Using icons and background colors to highlight key insights.
- KPI Indicators: Representing progress visually.
- Data Validation: Ensuring accuracy by cross-referencing with raw data.
- Power BI Desktop: Crafted interactive dashboards.
- SQL: For data sets and optimizing.
- Power BI Service: Publishing reports, setting up auto-refresh with a personal gateway, and managing access permissions.
- DAX Studio: Optimized performance for efficient reporting.
- Excel: Provided by stakeholders for reference User Acceptance Testing (UAT) report creation.

## 📝 Key Business Concepts Learned

This project also deepened my understanding of several key business terms, such as:

- Net Invoice Sales (NIS): Revenue after pre- and post-invoice deductions.
- Gross Margin: A measure of profitability.
- COGS (Cost of Goods Sold): Direct costs associated with producing goods.
- Gross Margin: Sales minus the cost of goods sold.
- Gross Margin %: Percentage of profit from sales.
- Market Share %: Company’s sales compared to the whole market.
- Forecast Accuracy: How close sales predictions are to actual sales.
- Net Error: Difference between actual and predicted results.
- Absolute Error: The exact difference between actual and predicted results.
- YTD (Year to Date) & YTG (Year to Go): Metrics to track progress over time.

## 🚀 Project Outcome

This dashboard has transformed how AtliQ Hardware approaches decision-making. Stakeholders can now answer critical questions backed by data, such as:

- Why are certain markets underperforming?
- Which products need more attention?
- How can we optimize inventory and reduce costs?
  
By implementing Power BI, AtliQ Hardware has taken the first step toward building a robust analytics culture, setting them up for success in a competitive market.

## 📂 Resources
- GitHub Repository: 
- Live Report: [[Business Insights 360](https://app.powerbi.com/links/23vrBin1Pf?ctid=c6e549b3-5f45-4032-aae9-d4244dc5b2c4&pbi_source=linkShare&bookmarkGuid=774945f8-0fab-4cc0-8879-c9da7d9954b0)]







