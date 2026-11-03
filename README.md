# Semicon-Sales-Analysis

## Executive Overview Dashboard

<img width="1600" height="905" alt="Dashboard 1 - Executive Overview" src="https://github.com/user-attachments/assets/7e525f0d-754b-4f30-8494-768fd10f9b2a" />

Purpose: Key details for Stakeholders

## Yearly Growth Dashboard

<img width="1601" height="900" alt="Dashboard 2 - Yearly Growth" src="https://github.com/user-attachments/assets/5519b7e1-75b4-4449-ad7c-ebb801e8ae73" />

Purpose: Showcasing Semicon's revenue-wise yearly performance

## All Links

**Live Dashboard Link:** [Click Here](https://public.tableau.com/views/SemiconSalesAnalysisDashboard/ExecutiveOverview?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Tools & Languages Used

* **Python & Jupyter Notebook** - Data Cleaning & Transformation
* **Microsoft Excel** - Data Organisation (Compiling each of the .csv files as separate sheets in a single workbook)
* **Tableau** - Data Analysis & Visualisation

## Background

Semicon sells computer hardware products through a customer base that includes brick-and-mortar and e-commerce sellers. Its transaction records span multiple products, customers, markets and dates. This project combines Python data preparation with a Tableau data model and interactive dashboards to make sales performance easier to review. The supplied dataset contains 50,000 transaction rows and four supporting tables for customers, dates, markets and products. Transactions cover October 2017 through June 2020. The Tableau model relates the transaction fact table to these four dimensions. Leadership and sales teams need a reliable view of sales scale, market performance, customer concentration, product contribution and monthly trends. Those questions are difficult to answer consistently when source fields contain formatting issues, multiple currencies and transaction values that require validation.

**Business questions include:**

* How much sales activity is represented by the data, and how do sales and quantities change by month and year?
* Which markets contribute the most sales value and units, and where is sales coverage limited?
* Which customers account for the largest share of sales, and how concentrated is the customer portfolio?
* Which products lead by sales value, and what products contribute most to performance?
* Can executives compare KPI cards and market, customer, product and time views using one consistent sales definition?

**Current reporting challenges include:**

* The five related tables must be cleaned and connected consistently before cross-market and time-based analysis can be trusted.
* Source text includes hidden whitespace and carriage returns, the customer-name field contains a typo, and some market zones are missing.
* Transactions include non-positive sales amounts and multiple currency codes. These records and currency conversions need documented rules.
* Business users need an executive overview as well as a separate view of monthly and year-level trends.
* The Tableau headline revenue measure multiplies converted sales amount by quantity, while several comparison charts sum converted sales amount. The intended business definition and calculation basis need to be reconciled.

## Data Model

<img width="605" height="389" alt="Data Model" src="https://github.com/user-attachments/assets/86ebe90c-5bef-49e0-8b18-0d7a987565e1" />

## Key Findings

### Market Performance
Delhi NCR is the largest market in the sales-amount view at INR 110.73M, followed by Mumbai at INR 58.09M, Ahmedabad at INR 49.62M and Nagpur at INR 37.85M. Mumbai leads units sold with 191.1K, slightly ahead of Delhi NCR at 183.2K. Comparing value with volume can help identify markets with different product or transaction mixes, but the dashboard does not provide margin or average selling-price analysis.

### Customer Concentration
Electricalsara Stores is the top customer at INR 73.90M in the dashboard ranking, followed by Excel Stores at INR 24.46M and Info Stores at INR 19.67M. The leading account contributes roughly 24% of the cleaned converted sales-amount total. This concentration supports closer account monitoring and a review of the sales mix behind the top account.

### Product Contribution
The top product in the sales-amount ranking is the Semicon Vortex V9-1200K Unlocked Desktop CPU at INR 23.58M. The next two shown are Semicon Titan DDR4 8GB 3600MHz Desktop RAM at INR 16.26M and Semicon Vortex V9-1200 Desktop CPU at INR 15.60M. CPU and memory products feature prominently among the leading products.

### Monthly and Annual Pattern
The monthly line chart shows its highest point in January 2018 at about INR 17.4M, followed by lower and uneven monthly results. A later high occurs in July 2019 at about INR 11.9M, while June 2020 is about INR 4.5M. Comparing complete years, converted sales amount falls from INR 123.35M in 2018 to INR 110.04M in 2019. The chart describes changes over time but does not explain their causes.

## Recommendations

* Reconcile the revenue definition first. Confirm the source meaning of sales_amount, then use one calculation and unit for every revenue KPI, trend and ranking. Add a reconciliation check to the workbook.
* Protect and review the largest accounts, beginning with Electricalsara Stores, and examine customer-level contribution over time to monitor concentration.
* Compare market sales value and unit volume together. Prioritise follow-up in leading markets such as Delhi NCR and Mumbai while reviewing lower-activity markets with local context.
* Review availability, pricing and promotion for the leading CPU and RAM products. The sales data identifies leaders but does not show inventory, margin or stock-out constraints.
* Investigate the 2018-2019 decline and uneven monthly changes with additional business context. Do not attribute the pattern to a cause based on this dashboard alone.
* Label partial years and the 96 INR/USD fixed conversion assumption directly in the report, and refresh the exchange rate when the analysis is updated.

## Conclusion
The project establishes a useful sales reporting foundation: cleaned transactions, linked product/customer/market/date dimensions, and dashboards that expose market, customer, product and time patterns. Its strongest immediate improvement is to reconcile and label the sales-value calculation. Once that is resolved, the dashboard can give leadership a consistent basis for monitoring sales performance and choosing where to investigate further.
