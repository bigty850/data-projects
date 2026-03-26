# E-Commerce Business Analytics: Conversion Funnel & Cohort Retention

## 📊 Project Overview
In this role as a Junior Analyst, I transformed raw e-commerce transaction logs into a strategic business report. The project focuses on analyzing user behavior through the conversion funnel—from product views to purchases—and measuring long-term customer loyalty using cohort retention analysis.

---

## 🎯 Business Objectives
* **Funnel Optimization:** Identify the drop-off rates between product views, cart additions, and final transactions.
* **Customer Acquisition Cohorts:** Group users by their first purchase month to track their behavior over a 4-month lifecycle.
* **Retention Analysis:** Calculate month-over-month retention rates to evaluate the store's ability to keep customers returning.
* **Data Engineering:** Clean and structure raw event logs using advanced spreadsheet functions to prepare them for executive-level insights.

---

## 🔍 Key Analysis Phases

### 1. Build a Conversion Funnel
Using a pivot table approach, I mapped the user journey across three distinct stages:
* **Stages:** Product View $\rightarrow$ Shopping Cart $\rightarrow$ Purchase.
* **Metrics:** Calculated **Total Conversion Rates** and **Step-to-Step Conversion Rates** to pinpoint where users lose interest in the purchasing process.

### 2. Data Preparation & Engineering
The core of this project involved cleaning and transforming raw data into a structured format for analysis:
* **Filtering:** Isolated purchase-specific events (approx. 4,845 rows) into a dedicated `purchase_activity` sheet.
* **First Purchase Logic:** Used `VLOOKUP()` and `MIN()` functions to identify the acquisition date for every unique user ID.
* **Feature Engineering:** * Created `event_month` and `first_purchase_month` using the `TEXT()` function (YYYY-MM).
    * Calculated `cohort_age` (0-4 months) using the `DATEDIF()` function to track user activity relative to their first purchase.

### 3. Cohort & Retention Rates
* **Cohort Analysis:** Aggregated data into **6 acquisition cohorts** based on the month of the user's first transaction.
* **Retention Matrix:** Built a retention table tracking the percentage of unique users from each cohort who returned in subsequent months (Ages 1-4).
* **Automated Calculations:** Leveraged fixed-column references to ensure the retention formula could be scaled across the entire matrix.

---

## 🛠️ Tools & Technical Skills
* **Advanced Spreadsheet Modeling:** Expert use of `VLOOKUP()`, `DATEDIF()`, `TEXT()`, and Pivot Tables.
* **Data Cleaning:** Filtering, data validation, and handling raw transaction logs.
* **Business Intelligence:** Funnel analysis, acquisition cohorting, and retention modeling.
* **Professional Documentation:** Created an **Executive Summary** and **Table of Contents** formatted for C-suite stakeholders.

---

## 📂 Project Structure
* `Executive Summary`: High-level results regarding funnel conversion and retention trends.
* `Table of Contents`: Document navigation and sheet descriptions.
* `Conversion Funnel`: Unique user counts and conversion rate calculations.
* `Retention Rates`: Final percentage-based cohort retention matrix.
* `Purchase Activity`: The cleaned dataset with all engineered time-dimensions.
* `Raw User Activity`: The original event logs spanning the full analysis period.
