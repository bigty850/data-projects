# VentureInsight: Exploring Startup Trends with SQL

## 📊 Project Overview
As a Data Analyst at **VentureInsight**, a leading research firm for venture capital, I conducted an in-depth analysis of a comprehensive database tracking the startup ecosystem. This project involved querying multi-relational databases to provide data-driven recommendations for multi-million dollar investment decisions.

---

## 🎯 Business Objectives
* **Market Baseline:** Calculate success vs. failure rates (closed vs. operating/acquired) in the startup landscape.
* **Sector Benchmarking:** Analyze funding trends for specific industries, such as the US media and news space, to help VC firms benchmark investment amounts.
* **Investor Profiling:** Categorize venture funds by activity level (High, Middle, Low) to identify potential co-investment partners.
* **Founder Analytics:** Examine the educational backgrounds of founders from failed startups to identify correlation patterns.

---

## 🔍 Key Technical Tasks & SQL Implementations

### 1. Startup Landscape Analysis
* **Objective:** Snapshot of the ecosystem's health.
* **Technical Skill:** Used `COUNT` aggregations with `WHERE` filters to isolate companies with a "closed" status.

### 2. Fund Activity Classification
To help clients find appropriate partners, I engineered a new categorical field using `CASE` logic:
* **High Activity:** 100+ companies invested.
* **Middle Activity:** 20–99 companies invested.
* **Low Activity:** < 20 companies invested.

### 3. Advanced Subqueries & Joins
I tackled complex business questions requiring nested logic, such as:
* **Founder Education Audit:** Wrote a multi-level subquery to find the average degree count for people associated with "closed" companies that only ever received a single round of funding.
* **Funding Trends:** Used `GROUP BY` and `HAVING` clauses to filter funding rounds by specific date ranges and investment amounts.

---

## 🛠️ Tools & SQL Concepts
* **Environment:** Relational Database (SQL).
* **Aggregations:** `SUM()`, `AVG()`, `COUNT()`, `MIN()`, `MAX()`.
* **Data Manipulation:** `CASE` statements for bucketed analysis and `JOIN` operations across 7+ tables (company, fund, funding_round, investment, acquisition, people, education).
* **Advanced Logic:** Multi-level subqueries and nested `SELECT` statements to bridge disparate data points like education and company status.

---

## 📂 Database Schema
The analysis was performed across a relational schema including:
* **Company:** Startup funding, status, and category.
* **Fund:** VC fund details and activity.
* **Funding_Round:** Detailed investment lifecycle data.
* **Acquisition:** Exit data and acquisition values.
* **Education:** Founder and employee academic backgrounds.

---

## 🏆 Key Achievement
* Successfully passed **10/10 auto-graded technical tasks** simulating real-world venture capital requests.
* Transformed raw relational data into actionable insights for quarterly investment reporting.
