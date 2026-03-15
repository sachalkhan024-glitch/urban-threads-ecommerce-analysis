# urban-threads-ecommerce-analysis
# 🛍️ Urban Threads E-Commerce Audit (Python EDA)

## 📌 Project Overview
Urban Threads, an online apparel retailer, recently ran an aggressive discount campaign. The objective of this analysis was to audit their messy transaction data, calculate true net revenue, and identify which product categories are actually driving profitable growth versus just moving empty volume.

## 🛠️ Tools & Methodology
* **Tools:** Python, Pandas, Matplotlib, Jupyter Notebook
* **Data Cleaning:** Handled missing/null discount values to prevent calculation errors and converted string-based dates into actionable datetime objects.
* **Feature Engineering:** Engineered a custom `Net_Revenue` metric applying the business logic: `(Price * Quantity) - Discount_Applied`.
* **Aggregation:** Utilized Pandas `.groupby()` to aggregate sales performance by product category and daily trends.

## 📈 Key Business Insights
1. **The Volume vs. Profit Trap:** While T-Shirts sold the highest absolute volume (12 units), they generated very low total revenue. **Joggers are the true profit engine**, driving $335 in Net Revenue (over 50% of the campaign's total) despite selling fewer units.
2. **Traffic Spikes:** Time-series analysis revealed a massive sales spike on March 3rd. Investigating the marketing channel attribution for this specific date could provide a blueprint for future campaigns.

## 💡 Strategic Recommendation
Shift ad spend and promotional focus away from T-Shirts and double down on Joggers. The data proves that driving traffic to the Joggers category yields a significantly higher Return on Investment (ROI).
