# Executive Retail Analytics Dashboard

![Executive Sales Overview](Images/ExecutiveDashboard.png)

## Executive Summary

This Power BI dashboard analyzes retail performance across sales, profit, customers, product categories, regions, and time. I built the report to give leadership a quick view of overall performance while still making it easy to move from the big picture into the areas driving those results.

Across the full reporting period, the business generated **$2.30M in sales** and **$286.40K in profit** from approximately **5,000 orders** and **793 customers**, resulting in a **12.47% profit margin** and an **average order value of $458.61**.

The strongest overall sales came from the **Technology** category, while the **West** led regional performance. Annual results were less consistent: sales declined in 2015 before recovering sharply in 2016 and continuing to grow in 2017.

## Performance Overview

The executive view brings the primary business measures into one place so overall performance can be reviewed without having to work through individual transaction records or separate reports.

### Key Results

| KPI | Result |
| --- | ---: |
| Total Sales | $2.30M |
| Total Profit | $286.40K |
| Total Orders | 5K |
| Total Customers | 793 |
| Profit Margin | 12.47% |
| Average Order Value | $458.61 |

Technology produced approximately **$0.84M in sales**, ahead of Furniture at **$0.74M** and Office Supplies at **$0.72M**. Regionally, the West generated approximately **$0.73M**, followed by the East at **$0.68M**. Central and South trailed the two leading regions, creating a clear difference in regional contribution.

The monthly view also shows that sales and profit do not always move at the same rate. Higher revenue does not automatically produce a proportional increase in profit, which makes profitability an important part of evaluating performance rather than relying on sales alone.

## Year-over-Year Performance

The second page focuses on how the business changed from year to year. Selecting a year updates profit margin, year-over-year sales growth, category results, customer segment mix, monthly sales, and monthly profit so each period can be evaluated in the same context.

### 2015 Performance

![2015 Sales Trends and Performance](Images/SalesTrends2015.png)

Sales declined **2.83% year over year in 2015**, while profit margin finished at **13.10%**. The monthly results show an uneven year, with stronger sales late in the period helping offset weaker performance earlier in the year.

### 2016 Performance

![2016 Sales Trends and Performance](Images/SalesTrends2016.png)

Performance changed considerably in 2016. Sales increased **29.47% year over year**, the strongest annual growth in the reporting period, while profit margin improved to **13.43%**. Sales strengthened during the second half of the year and finished with particularly strong results in the final months.

Growth continued into 2017 at **20.36%**, although profit margin decreased to **12.74%**. Taken together, the annual results show a business that recovered strongly from the 2015 decline while still requiring attention to the relationship between revenue growth and profitability.

## Business Insights

Several findings stand out across the report:

- **Technology leads category sales**, making it the largest revenue contributor across the full reporting period.
- **West and East lead regional sales**, while Central and South represent the weaker regional results.
- **Consumer is the largest customer segment**, accounting for the greatest share of sales in the yearly views.
- **2015 was the only year with negative year-over-year growth** in the available comparison period.
- **2016 produced the strongest annual recovery**, with sales growth of 29.47% and the highest profit margin among the displayed yearly views.
- **Revenue and profit do not move proportionally every month**, making margin and profit performance necessary alongside sales when evaluating results.

## Business Use

The report is designed to support common management questions without requiring separate analysis for each one. It can be used to review overall business performance, identify leading categories and regions, compare annual results, examine customer segment contribution, and isolate months where sales or profitability changed materially.

The year-level view also makes it possible to move from an overall result into the underlying monthly and category performance without changing reports. This keeps the executive summary and the supporting analysis connected.

## Power BI Development

I built the project in Microsoft Power BI using the Sample Superstore dataset. The model includes a dedicated Date Table to support monthly reporting and year-over-year comparisons, along with reusable DAX measures separated from the raw dataset.

Key measures developed for the report include:

- Total Sales
- Total Profit
- Total Orders
- Total Customers
- Average Order Value
- Profit Margin
- Year-over-Year Sales Growth %

The report also uses filter context, time-intelligence calculations, interactive slicing, and conditional formatting to keep the analysis responsive as the selected reporting period changes. For 2014, year-over-year growth is intentionally unavailable because the dataset does not contain the prior-year data required for a valid comparison.

## Tools & Skills

**Power BI · Power Query · DAX · Data Modeling · Data Cleaning · Time Intelligence · KPI Development · Interactive Reporting · Data Visualization · Business Analysis · Git · GitHub**

## Dataset

The analysis uses the **Sample Superstore** retail dataset, which contains order-level information covering sales, profit, customers, products, categories, discounts, shipping, dates, and geographic regions.

The source data is included in the `Data` directory for reproducibility.

## Repository Structure

```text
executive-retail-analytics-dashboard/
├── README.md
├── ExecutiveRetailAnalyticsDashboard.pbix
├── Images/
│   ├── ExecutiveDashboard.png
│   ├── SalesTrends2014.png
│   ├── SalesTrends2015.png
│   ├── SalesTrends2016.png
│   └── SalesTrends2017.png
└── Data/
    └── Sample - Superstore.csv
```

## Project Status

**Completed — August 2026**

The final report contains an Executive Sales Overview and an interactive Sales Trends & Performance page covering all four years available in the dataset.

## Author

### Jesse Luffman

Data analytics professional and Bachelor of Information Technology student focused on using data to answer practical business questions and communicate the results clearly through business intelligence and analytics tools.
