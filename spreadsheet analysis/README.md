# Manhattan Airbnb Investment Analysis: Data-Driven Real Estate Insights

## 📊 Project Overview
This project involves a comprehensive analysis of the Manhattan vacation rental market using Airbnb data. The goal was to provide strategic guidance to a client looking to invest in Manhattan properties by identifying the most "attractive" neighborhoods and property sizes based on rental frequency and revenue potential.

---

## 🎯 Business Objectives
* **Market Attractiveness:** Define and measure "attractiveness" using the number of reviews in the last 12 months (LTM) as a proxy for booking frequency.
* **Property Optimization:** Identify which property sizes (studios, 1-bedroom, etc.) perform best in specific high-demand neighborhoods.
* **Revenue Forecasting:** Estimate annual revenue for top-performing listings by analyzing 30-day price fluctuations and availability data.
* **Investment Recommendation:** Narrow down a vast dataset into a high-priority "Top Listing" list for the client.

---

## 🔍 Key Insights & Analysis

### 1. Neighborhood & Size Popularity
* **Data Cleaning:** Cleaned the `neighborhood` column to remove inconsistent capitalization and trailing spaces. Standardized the `bedrooms` column by converting empty cells into "Studios" (0 bedrooms) using `IF` logic.
* **Top 10 Neighborhoods:** Built pivot tables to rank neighborhoods by total reviews. Key hotspots identified include **Harlem**, **Midtown**, and the **Upper West Side**.
* **The "Sweet Spot":** Discovered that **1-bedroom** apartments are the most popular across almost all top neighborhoods, except for **Midtown**, where **studios** dominate the market.

### 2. Financial Modeling
* **Revenue Logic:** Developed a custom `revenue_earned` metric in the calendar dataset. 
    * *Logic:* If a property was marked as "not available" (`f`), the daily `adjusted_price` was recorded as revenue; otherwise, it was $0.
* **Annual Projections:** Aggregated 30-day revenue to the `listings` level using `SUMIF()`. Projected annual earnings by applying a 12x multiplier to the 30-day baseline.
* **Top Performer:** Identified a single top-earning listing that generated **$29,940** in a single 30-day period.

---

## 🛠️ Tools & Technical Skills
* **Excel Functions:** `SUMIF()`, `IF()`, `VLOOKUP()`, and complex arithmetic formulas for revenue forecasting.
* **Data Engineering:** Created a "Change Log" to document all cleaning steps (capitalization, whitespace removal, and null-value handling).
* **Data Visualization:** Generated pivot tables and bar charts to compare neighborhood performance and property size preferences.
* **Business Communication:** Produced an **Executive Summary** and **Table of Contents** to translate raw data into a professional investment brief.

---

## 📂 Project Structure
* `Executive Summary`: High-level investment advice and key findings.
* `Data Cleaning Log`: A step-by-step record of data transformations from raw state to clean state.
* `Analysis Sheets`: Pivot tables and charts broken down by neighborhood and bedroom count.
* `Revenue Model`: Detailed breakdown of projected monthly and annual earnings.
* `Raw Data`: Untouched original Airbnb dataset for Manhattan.
