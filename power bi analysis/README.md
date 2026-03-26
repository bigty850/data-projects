# Shopify App Store Analysis: Success Factors & Developer Engagement

## 📊 Project Overview
This project provides a comprehensive audit of the Shopify App Store ecosystem. Using data scraped from public Shopify listings, I built a multi-page Power BI report to identify the key factors—such as review volume, rating quality, and developer responsiveness—that drive an app's success and visibility on the platform.

---

## 🎯 Business Objectives
* **Landscape Mapping:** Quantify the scale of the marketplace and track review trends over time.
* **Sentiment & Quality Correlation:** Analyze the relationship between the volume of reviews and average user ratings.
* **Engagement Metrics:** Measure how developer interaction (replies to reviews) correlates with higher app ratings.
* **Developer Benchmarking:** Identify top-performing and most responsive developers using weighted "Helpfulness" metrics.

---

## 🔍 Key Insights & Visualizations

### Part 1: App Landscape
* **Market Scale:** Used **KPI Cards** to track the unique count of apps within the dataset.
* **Trend Analysis:** A **Line Chart** of review totals over time (`lastmod` date) highlights periods of peak user activity and platform growth.
* **Quality vs. Quantity:** A **Scatterplot** comparing review counts to average ratings revealed whether high-volume "popular" apps maintain quality compared to niche offerings.

### Part 2: Advanced DAX & Review Weighting
I utilized Data Analysis Expressions (DAX) to create more nuanced performance metrics:
* **Helpfulness Score:** Created a calculated column `helpful_reviews` using the formula:  
    `rating * (1 + helpful_count)`  
    This ensures that highly-voted reviews carry more weight in the final analysis.
* **Response Logic:** Engineered a binary `developer_answered` column to track which reviews received a reply, allowing for a direct comparison of ratings between engaged and unengaged developers.

### Part 3: Developer Performance & Responsiveness
* **Data Modeling:** Established a **Many-to-One relationship** between the `Reviews` and `Apps` tables to aggregate user sentiment at the developer level.
* **Refined Metrics:** Moved beyond simple "Sum of Ratings" to "Average Helpful Review" to eliminate bias toward apps that simply have a high volume of low-quality reviews.
* **Responsiveness Leaderboard:** Built a filtered bar chart identifying the most active developers among high-traffic apps (those with >500 reviews).

---

## 🛠️ Tools & Technical Skills
* **Power BI Desktop:** Report authoring, visualization design, and interactive filtering.
* **DAX (Data Analysis Expressions):** Created custom calculated columns for weighted averages and conditional logic.
* **Data Modeling:** Built relational schemas between app metadata and user review tables.
* **Market Research:** Interpreted scatterplot distributions to provide actionable business advice for prospective app developers.

---

## 📂 Project Structure
* **App Landscape:** High-level market statistics and time-series data.
* **Reviews Analysis:** Deep dive into user sentiment and DAX-driven helpfulness metrics.
* **App Reviews / Developer Performance:** Competitive analysis and responsiveness tracking.
