# Superstore Profitability Analysis: Data Visualization with Tableau

## 📊 Project Overview
The Superstore is facing a financial crisis and is on the brink of bankruptcy[cite: 1]. This project serves as a strategic consultancy audit to identify significant profit centers, eliminate chronic loss-makers, optimize advertising spend, and analyze the impact of product returns on the bottom line.

**🔗 [View the Interactive Tableau Workbook Here](INSERT_YOUR_TABLEAU_PUBLIC_LINK_HERE)**

---

## 🎯 Business Objectives
* **Profit & Loss Audit:** Identify the dimensions (Sub-category, Shipping Mode, etc.) driving the highest gains and deepest losses.
* **Inventory Optimization:** Determine specific products and sub-categories that should be discontinued based on negative profit margins.
* **Strategic Advertising:** Calculate the Return on Ad Spend (ROAS) to identify the top state-month combinations for marketing investment[cite: 217, 218, 219].
* **Returns Analysis:** Quantify return rates by product and customer to mitigate revenue leakage[cite: 237, 239].

---

## 🔍 Key Insights & Visualizations

### Part 1: Profits & Losses
* **Profit Centers:** Analysis of Sub-category and Shipping Mode combinations revealed the most lucrative segments[cite: 1].
* **Loss Mitigation:** The "Cubify CubeX 3D Printer" and various tables/bookcases were identified as significant loss-makers[cite: 7]. 
* **Strategic Focus:** Recommended focusing on the three best subcategories (Copiers, Phones, and Accessories) while stopping sales for the worst three (Tables, Bookcases, and Supplies)[cite: 13, 19].

### Part 2: Advertising Optimization
Based on a target of spending 1/5 of profits on advertising, the following state/month combinations are the most viable[cite: 217, 218, 219]:
| State | Month | Profit | Recommended Ad Budget |
| :--- | :--- | :--- | :--- |
| **Indiana** | October | $643.10 | [cite_start]**$128.62** [cite: 217] |
| **Vermont** | November | $596.00 | [cite_start]**$119.20** [cite: 218] |
| **Washington** | March | $521.30 | [cite_start]**$104.26** [cite: 219] |

### Part 3: Product Returns
* **Data Engineering:** Created a calculated field to normalize Return data where "Yes" values are 1 and "Null" values are 0[cite: 1].
* **Performance Tracking:** Visualized return rates by customer and product to identify outliers[cite: 239, 240]. **Correlation:** Analyzed Average Profit against Average Return Rate to determine which dimensions provide a sustainable return on investment versus those that are too costly to maintain[cite: 257, 258].

---

## 🛠️ Tools Used
* **Tableau Desktop:** For advanced data visualization and dashboarding.
* **Excel:** Initial data source (`Superstore.xls`).
* **Data Modeling:** Performed LEFT JOINs between Order and Return tables to ensure data integrity[cite: 1].

---

## 📂 Project Structure
* `README.md`: Project summary and strategic insights.
* `Superstore_Project.pdf`: Static export of the Tableau dashboards.
* `Superstore_Analysis.twbx`: Packaged Tableau workbook (available via Tableau Public link).
