# Superstore-Sales-Business-Intelligence
# Superstore Sales Business Intelligence Project

## Project Overview

This project uses Microsoft Power BI to analyse the Sample Superstore sales dataset and turn transaction-level data into practical business information. The analysis examines sales, profitability, product and category performance, customer segments, regional performance and changes in sales over time.

The project was completed as part of the AnalystLab Africa Week 2 Business Analytics Case Study.

## Project Objectives

- Assess overall sales and profitability.
- Compare performance across product categories and sub-categories.
- Examine sales across regions, states and customer segments.
- Review monthly sales performance over the available period.
- Identify business risks and opportunities.
- Develop recommendations to support better commercial and operational decisions.

## Dataset

The project uses the **Sample - Superstore** dataset.

| Dataset characteristic | Description |
|---|---:|
| Transaction records | 9,994 |
| Columns | 21 |
| Distinct orders | 5,009 |
| Distinct customers | 793 |
| Distinct products | 1,862 |
| Period covered | 2014–2017 |

The dataset contains order dates, shipping dates, customer and geographic details, product categories and sub-categories, sales, quantities, discounts and profit.


## Data Preparation

Data preparation was carried out in Power Query before the data was used in Power BI.

Key checks and transformations included:

- Reviewed the dataset structure and assigned appropriate data types.
- Set Order Date and Ship Date to the Date data type.
- Set numerical fields such as Sales, Discount and Profit to appropriate numeric types.
- Checked for missing values and blank rows.
- Checked for exact duplicate records across all 21 columns. The check returned zero exact duplicate rows.
- Checked for negative and zero sales values and discounts outside the expected 0–1 range. No such records were identified.
- Compared Order Date and Ship Date. No records had a shipping date earlier than the order date.
- Identified negative-profit transactions and retained them because they represent potentially valid business outcomes rather than automatic data errors.

The dataset contains 1,871 transaction records with negative profit (18.72% of transaction rows). These were retained so that loss-making activity remained visible in the analysis.

## Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Sales | $2,297,200.86 |
| Total Profit | $286,397.02 |
| Total Orders | 5,009 |
| Average Order Value | $458.61 |
| Profit Margin | 12.47% |

Total Orders is based on distinct Order IDs rather than transaction rows. Average Order Value is calculated as total sales divided by distinct orders.

## Power BI Dashboard

The Power BI report contains two pages.

### 1. Executive Sales Overview

This page provides a high-level view of sales performance through KPI cards and visuals covering:

- Sales by region
- Sales by category
- Monthly sales trend
- Sales distribution by customer segment
- Sales performance by state

### 2. Product and Profitability Analysis

This page focuses on product performance and profitability, including:

- Profit by sub-category
- Profit by category
- Category and sub-category performance matrix
- Sales, profit and profit margin comparisons

The report includes slicers for **Year, Region, Category and Segment** to allow users to explore the results interactively.

## Key Business Findings

### 1. Technology leads in sales and profit

Technology generated the highest category sales at **$836,154.03** and the highest category profit at **$145,454.95**, with a profit margin of approximately **17.40%**.

### 2. Furniture has a profitability challenge

Furniture generated **$741,999.80** in sales but only **$18,451.27** in profit, giving it a margin of approximately **2.49%**. This indicates that strong sales volume does not necessarily translate into strong profitability.

### 3. Office Supplies has the lowest category sales but a healthy margin

Office Supplies recorded **$719,047.03** in sales and **$122,490.86** in profit, with a margin of approximately **17.04%**.

### 4. Profitability differs considerably by sub-category

Copiers recorded a profit margin of approximately **37.19%**, while Machines recorded approximately **1.79%**. Tables, Bookcases and Supplies recorded negative profit margins of approximately **-8.56%**, **-3.02%** and **-2.55%**, respectively.

### 5. Customer sales are concentrated in the Consumer segment

Consumer customers contributed approximately **50.56%** of total sales, followed by Corporate customers at **30.74%** and Home Office customers at **18.70%**.

The monthly sales trend fluctuates over the period analysed, with increases and declines rather than a consistently rising pattern.

## Risks and Opportunities

### Risks

- **Low Furniture profitability:** The category's margin is substantially lower than those of Technology and Office Supplies.
- **Loss-making sub-categories:** Negative margins in Tables, Bookcases and Supplies warrant further investigation.
- **Uneven customer-segment contribution:** The Consumer segment accounts for just over half of sales, making it important to retain this customer base while developing other segments.

### Opportunities

- **Expand high-margin product lines:** Copiers and Accessories offer opportunities for carefully targeted growth, subject to demand and stock availability.
- **Improve product-level profitability:** Reviewing pricing, discounts, supplier costs and product strategy may help improve weak-performing categories and sub-categories.
- **Develop Corporate and Home Office sales:** Targeted offers and relationship-building could grow these segments while maintaining Consumer customer retention.

## Recommendations

1. **Review Furniture profitability.** Examine product-level pricing, discounting, supplier costs and other relevant costs, particularly for Tables and Bookcases.
2. **Investigate loss-making sub-categories.** Review Tables, Bookcases and Supplies to understand the drivers of negative margins before deciding whether pricing, discount or product changes are appropriate.
3. **Support high-margin products.** Consider targeted sales activity for Copiers and Accessories while monitoring demand, stock availability and realised profitability.
4. **Develop customer segments.** Build targeted engagement and retention initiatives for Corporate and Home Office customers without neglecting the Consumer segment.
5. **Use monthly performance for planning.** Compare monthly results across the four-year period to inform sales targets, inventory, staffing and promotional planning. Further analysis would be needed before treating any recurring pattern as seasonality.

## Repository Contents

The repository should is organised as follows:

```text
superstore-sales-business-intelligence/
├── README.md
├── reports/
│   ├── Business_Intelligence_Report.pdf
│   └── Executive_Summary.pdf
├── power-bi/
│   └── Superstore_Sales_Analysis.pbix
├── dashboard/
│   ├── Dashboard_Export.pdf
│   └── Dashboard_Overview.png
└── data/
    └── README.md
```

## Project Files and Access

- **Business Intelligence Report:** `reports/Business_Intelligence_Report.pdf`
- **Executive Summary:** `reports/Executive_Summary.pdf`
- **Dashboard Export:** `dashboard/Dashboard_Export.pdf`
- **Power BI Project:** `power-bi/Superstore_Sales_Analysis.pbix`
- **Google Drive submission folder:** https://drive.google.com/drive/folders/1PFz1FARk7PUk6b9qlZ-EfcvhsXmzDyRT?usp=drive_link
- **Power BI file (if hosted separately):** https://drive.google.com/file/d/1SKb9Pi-C8lzttrx_8hBNKxRDofUFI539/view?usp=drive_link

## Tools Used

- Microsoft Power BI
- Power Query
- Microsoft Excel
- GitHub

## Conclusion

This project demonstrates how business intelligence tools can transform sales data into information that supports business decisions. The analysis shows positive overall profitability, but also highlights meaningful differences in performance across categories, sub-categories and customer segments. The recommendations focus on improving weak margins, supporting profitable products, developing customer segments and using performance trends to strengthen planning.

---

**Project:** AnalystLab Africa – Week 2 Business Analytics Case Study  
**Dataset:** Sample - Superstore  
**Author:** Shammah Muneta
