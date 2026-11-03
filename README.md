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









