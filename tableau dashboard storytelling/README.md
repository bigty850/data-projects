# Superstore Returns Analysis: Root Cause Identification & Executive Reporting

## 📊 Project Overview
High return rates can silently erode the profitability of even the most successful retail operations. In this project, I acted as a lead analyst tasked with identifying the "why" behind returned orders at the Superstore. I developed a comprehensive Tableau Story to help the CEO understand return drivers and implemented a monitoring dashboard to track these metrics in real-time.

---

## 🎯 Business Objectives
* **Root Cause Identification:** Determine if returns are driven by specific product categories, geographic regions, or seasonal trends.
* **Customer Profiling:** Identify "high-return" customers to understand behavioral patterns.
* **Dashboard Engineering:** Build a sustainable monitoring tool that allows stakeholders to filter by dimensions and drill down into specific loss-centers.
* **Data Storytelling:** Present findings in a structured "Story Arc" that moves from a high-level summary to specific, actionable recommendations.

---

## 🔍 Analytical Approach & Insights

### 1. Data Engineering & Modeling
* **Joins:** Performed a **LEFT JOIN** between the `Orders` and `Returns` tables.
* **Calculated Metrics:** Created a binary `Returned` field (1 for "Yes", 0 for "Null") to calculate the **Return Rate** (Average of the field) and **Total Returns** (Sum of the field).

### 2. Root Cause Analysis
* **Sales vs. Returns Correlation:** Developed a scatterplot by sub-category to determine if high sales volume inherently leads to high returns.
* **Geographic Concentration:** Created a map visualization to identify "Return Hotspots"—states or cities where logistics or regional preferences may be impacting satisfaction.
* **Seasonality:** Analyzed return rates over time (Month/Week) to detect spikes following holiday seasons or specific promotional periods.
* **Composite Factors:** Built multi-dimensional charts to see how geography and product category intersect (e.g., "Are Furniture returns higher in the West region?").

---

## 🎨 Dashboard Design & Storytelling
This project followed a full design lifecycle:
1.  **Low-Fidelity Wireframing:** Created 3 pen-and-paper mockups to iterate on user experience (UX) and layout before building in Tableau.
2.  **Dashboard Template:** Developed a layout using empty containers to ensure a polished, professional structure.
3.  **Tableau Story:** Constructed a narrative for the CEO including:
    * **Summary of Returns:** Defining the best measure of success (Rate vs. Total Count).
    * **Key Root Causes:** Direct answers to the "Why."
    * **Interactive Demo:** Instructions on how the CEO can use the dashboard filters to find specific issues.
    * **Proposed Next Steps:** Actionable items to reduce return volume.

---

## 🛠️ Tools & Technical Skills
* **Tableau Desktop:** Advanced dashboarding, Story Points, and mapping.
* **Data Modeling:** Left joins and calculated fields.
* **UX/UI Design:** Wireframing, mockup iteration, and dashboard templating.
* **Executive Presentation:** Structuring a 3-5 minute presentation aimed at C-suite stakeholders.

---

## 📂 Project Structure
* `Return_Analysis_Story.twbx`: Complete Tableau Packaged Workbook including the analysis, dashboard, and story arc.
* `Design_Process/`: Folder containing scans of pen-and-paper mockups and dashboard templates.
* `Presentation_Summary.pdf`: A PDF version of the final presentation slides and recommendations.
