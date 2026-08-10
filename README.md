# Executive Retail Analytics Dashboard

![Executive Sales Overview](Images/ExecutiveDashboard.png)

> A two-page Power BI business intelligence dashboard designed to turn retail transaction data into an executive overview and an interactive year-by-year performance analysis.

## Project Overview

This project uses the Sample Superstore dataset to demonstrate an end-to-end Power BI workflow: data preparation, modeling, DAX measures, KPI development, time intelligence, interactive filtering, and dashboard design.

The report is built around two complementary views:

- **Executive Sales Overview** — a high-level summary of overall business performance.
- **Sales Trends & Performance** — an interactive year-level analysis of sales growth, profitability, category performance, customer segments, and monthly trends.

The goal was not simply to display charts, but to create a report that a business leader could scan quickly and then use to investigate changes in performance.

## Dashboard Highlights

The Executive Sales Overview summarizes the full dataset with six headline KPIs:

| KPI | Result |
| --- | ---: |
| Total Sales | $2.30M |
| Total Profit | $286.40K |
| Total Orders | 5K |
| Total Customers | 793 |
| Profit Margin | 12.47% |
| Average Order Value | $458.61 |

It also compares sales across product categories and regions and shows the relationship between monthly sales and profit across 2014–2017.

## Interactive Sales Trends & Performance

The second report page adds a year slicer for 2014–2017 and updates the report dynamically. It includes:

- Profit Margin KPI
- Year-over-Year Sales Growth KPI
- Conditional KPI formatting for positive and negative YoY growth
- Sales and Profit by Category
- Sales by Customer Segment
- Monthly Sales Trend
- Monthly Profit

For 2014, YoY growth is intentionally displayed as unavailable because no prior-year comparison exists.

## Key Findings

- **Technology** generated the highest overall sales among the three product categories.
- The **West** was the strongest region by total sales, followed by the East.
- Overall performance reached approximately **$2.30M in sales** and **$286.4K in profit**, producing a **12.47% profit margin**.
- Sales declined **2.83% year over year in 2015** before rebounding strongly with **29.47% growth in 2016**.
- Growth remained positive in 2017 at **20.36%**, showing that the 2016 recovery continued into the following year.
- Consumer customers represented the largest share of sales across the yearly segment views.
- Monthly sales and monthly profit do not always move proportionally, reinforcing the importance of monitoring profitability alongside revenue.

## Business Questions Addressed

This dashboard was designed to answer questions such as:

- How is the business performing overall?
- Which product categories generate the most revenue and profit?
- Which geographic regions lead sales performance?
- How have sales and profit changed over time?
- Is annual sales performance improving or declining compared with the previous year?
- Which customer segments contribute the largest share of sales?
- Which months show unusually strong or weak performance?

## Data Model & DAX

A dedicated Date Table supports monthly analysis and year-over-year calculations. Reusable measures were organized separately from raw fields to keep the model easier to maintain.

Core measures include:

- Total Sales
- Total Profit
- Total Orders
- Total Customers
- Average Order Value
- Profit Margin
- YoY Sales Growth %

The YoY measure compares the selected year's sales against the prior year and feeds conditional formatting on the KPI card so declines appear red and positive growth appears green.

## Design Approach

The visual design uses consistent semantic colors across both pages:

- **Blue** represents sales.
- **Green** represents profit and positive performance.
- **Red** identifies negative year-over-year growth.
- Neutral gray/black styling is used for the primary year-selection control.

The report uses aligned visual containers, consistent typography, KPI cards, simplified axis labeling, and restrained formatting to keep the focus on the business information.

## Tools & Skills Demonstrated

- Microsoft Power BI
- Power Query
- DAX / Time Intelligence
- Data Cleaning & Transformation
- Data Modeling
- Date Table Development
- KPI Design
- Conditional Formatting
- Interactive Slicers
- Business Intelligence Reporting
- Data Visualization
- Analytical Storytelling
- Git & GitHub

## Dataset

The project uses the **Sample Superstore** retail dataset, containing order-level information including customers, products, categories, sales, profit, discounts, shipping information, dates, and geographic regions.

The dataset is included in the `Data` directory for reproducibility.

## Repository Structure

```text
executive-retail-analytics-dashboard/
├── README.md
├── ExecutiveRetailAnalyticsDashboard.pbix
├── Images/
│   └── ExecutiveDashboard.png
└── Data/
    └── Sample - Superstore.csv
```

## Project Status

**Portfolio-ready dashboard — completed August 2026.**

The current version contains the finished Executive Sales Overview and Sales Trends & Performance pages and has been reviewed across all four available years to verify filtering, KPI behavior, conditional formatting, and visual scaling.

## Author

### Jesse Luffman

Data analytics professional and Bachelor of Information Technology student focused on building practical business intelligence and analytics projects with Power BI, SQL, Excel, and related data tools.
