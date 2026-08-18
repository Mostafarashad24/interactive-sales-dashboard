# Data Analytics Project 4

## Project Overview

This project transforms a cleaned e-commerce sales-order dataset into an interactive Microsoft Excel dashboard.

The main business question is:

> Which products and referral sources contribute most to recorded sales value, and where should sales efforts focus?

The workbook combines data cleaning, validation, calculated analysis, and interactive visualizations to examine recorded order value across products, referral sources, and months.

## Objectives

- Prepare and validate the sales-order dataset for analysis.
- Analyze recorded order value by product.
- Compare recorded order value across referral sources.
- Examine monthly recorded order value over time.
- Provide an interactive dashboard for filtering the analysis.
- Present the main findings through clear, decision-oriented visualizations.

## Dataset

The project uses an e-commerce sales-order dataset containing 1,200 cleaned records and 14 columns.

Important fields include:

- `OrderID`
- `Date`
- `CustomerID`
- `Product`
- `Quantity`
- `UnitPrice`
- `ShippingAddress`
- `PaymentMethod`
- `OrderStatus`
- `TrackingNumber`
- `ItemsInCart`
- `CouponCode`
- `ReferralSource`
- `TotalPrice`

The cleaned dataset retains all 1,200 records.

The workbook defines `TotalPrice` as recorded order value. Cancelled and Returned orders are included, so recorded order value should not automatically be interpreted as net or realized revenue.

## Analysis Performed

### Data Cleaning and Validation

The workbook includes dedicated cleaning and validation documentation.

The cleaning checks confirm:

- 1,200 rows
- 14 columns
- 0 missing values after cleaning
- 0 missing `CouponCode` values after replacing blank values with `No Coupon`
- 0 duplicate rows
- 0 duplicate `OrderID` values
- 0 invalid or missing dates

### Product Analysis

Recorded order value and order count are calculated for each product.

The analysis covers:

- Chair
- Printer
- Laptop
- Tablet
- Monitor
- Desk
- Phone

Chair has the highest recorded order value at 195,620.11, followed closely by Printer at 195,612.61.

### Referral Source Analysis

Recorded order value and order count are also analyzed by referral source.

The referral sources include:

- Instagram
- Email
- Google
- Facebook
- Referral

Instagram has the highest recorded order value at 275,285.45, followed by Email at 261,808.55.

### Monthly Analysis

The workbook calculates recorded order value by month from January 2023 through June 2025.

The monthly analysis is used to identify peaks and dips in recorded order value rather than automatically interpreting them as long-term growth.

## Key Findings

- Total recorded order value across the dataset is 1,264,761.96.
- The dataset contains 1,200 orders.
- Average recorded order value is 1,053.9683.
- Total quantity across the dataset is 3,535.
- Chair leads the product analysis with 195,620.11 in recorded order value.
- Printer is very close behind Chair with 195,612.61.
- Instagram leads the referral-source analysis with 275,285.45 in recorded order value.
- Email follows Instagram with 261,808.55.
- The dashboard's documented takeaway recommends prioritizing strong product contributors, investigating weaker products, and examining Instagram and Email for repeatable acquisition patterns.
- The workbook specifically recommends investigating peak months by product and referral source before making claims about growth.

## Visualizations / Dashboard

The `Dashboard` worksheet contains an interactive dashboard with three main visualizations:

1. **Product revenue bar chart** — compares recorded order value across products, highlighting Chair and Printer as leading contributors.
2. **Referral-source revenue bar chart** — compares recorded order value across referral sources, with Instagram and Email leading the analysis.
3. **Monthly recorded order value line chart** — shows peaks and dips in recorded order value over time from 2023 through 2025.

The dashboard also contains four dropdown filters:

- Product
- Referral Source
- Order Status
- Year

The KPI section dynamically displays:

- Orders
- Recorded Order Value
- Average Order Value
- Quantity

The dashboard includes a visible "So What?" section summarizing the recommended interpretation of the analysis.

## Tools

- Microsoft Excel

## Workbook Structure

- `Dashboard` — Interactive dashboard containing KPIs, three visualizations, filters, and the main analytical takeaways.
- `Analysis` — Filtered calculations supporting product, referral-source, and monthly analysis.
- `README` — Project purpose, business question, visualization details, data notes, quality checks, and design checks.
- `Cleaned Data` — Cleaned 1,200-row dataset used by the dashboard and analysis.
- `Raw Data` — Original dataset before the documented cleaning process.
- `Cleaning Report` — Documents row/column counts and data-quality checks.
- `Evidence` — Validation evidence confirming the cleaning checks passed.

## Project Outcome

The completed project turns the cleaned sales-order data into an interactive Excel dashboard that makes product, referral-source, and monthly recorded order value easier to compare.

The analysis identifies Chair as the leading product by recorded order value and Instagram as the leading referral source. The dashboard allows these results to be explored interactively by product, referral source, order status, and year while clearly distinguishing recorded order value from net or realized revenue.

## Project Files

```text
.
├── data/
│   └── Project4_Interactive_Excel_Dashboard_Mostafa_Mahmoud_FINAL.xlsx
├── README.md
└── .gitignore
