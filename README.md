# Vrinda Store Sales Dashboard

## What This Is

A Power BI dashboard built to make sense of Vrinda Store's 2022 sales data. The store sells across 7 platforms — Amazon, Flipkart, Myntra, Ajio, Meesho, Nalli, and a few others — so having everything in one place made it a lot easier to see what was actually going on with revenue, returns, and who's buying what.

## Tech Stack

- **Power BI Desktop** — main tool for building the dashboard and writing DAX measures
- **Microsoft Excel (.xlsx)** — where the raw data lives
- **Power Query (M)** — used to clean and shape the data before loading it in
- **Bing Maps (Power BI visual)** — to plot revenue across Indian states on a map

## Data Source

Everything comes from a single Excel file, `Vrinda_Store.xlsx`, with just one sheet — `Vrinda Store`. It has 31,047 rows and 21 columns covering the full year from January to December 2022.

| Field | What It Holds |
|---|---|
| `Order ID`, `Cust ID`, `SKU` | Identifiers for orders, customers, and products |
| `Gender`, `Age`, `Age Group` | Customer info — age groups are Adult, Teenager, and Senior |
| `Date`, `Month` | When the order was placed |
| `Status` | Whether it was Delivered, Cancelled, Returned, or Refunded |
| `Channel` | Which platform the order came from |
| `Category`, `Size`, `Qty` | Product details — categories include Kurta, Set, Western Dress, Top, Saree, Blouse, Ethnic Dress, and Bottom |
| `Amount`, `currency` | Order value in INR |
| `ship-city`, `ship-state`, `ship-postal-code`, `ship-country` | Delivery location — covers 50 states and 2,600+ cities across India |
| `B2B` | Whether the buyer was a business or an individual |

Excel File directly connected to Power BI.

## What the Dashboard Covers

The report has three pages, each looking at things from a different angle.

**Page 1 — Sales & Demographics**

This page answers the basic questions: what's selling, and who's buying it? Women placed significantly more orders than men (21,553 vs 9,494), Adults are the biggest age group, and Sets along with Kurtas drive the most revenue. There's a treemap, a bar chart breaking down revenue by product, and donut and column charts for gender and age group splits. You can slice by Category or Gender to dig into specifics.

**Page 2 — Fulfillment & Returns**

The headline number here is a 92% fulfillment rate, which is solid. Cancellations sit at 3% and refunds at 2%. Amazon has the highest number of cancelled deliveries by a notable margin, and the trend line shows returns climbing toward the end of the year — something worth keeping an eye on heading into the next year.

**Page 3 — Revenue & Geography**

Total revenue for 2022 came in at ₹21M across 28K orders, with an average order value of ₹682. Revenue peaked early in the year and gradually declined through Q3 and Q4. Amazon leads on order volume, followed by Myntra and Flipkart. The map shows which Indian states contributed the most revenue.

All three pages share the same slicers — Category, Gender, Channel, and Status — so filtering on one page carries context across the whole report.
