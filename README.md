# 🗽 NYC Airbnb Market Analysis & Data Cleaning

## 📌 Project Overview
This project analyzes the New York City Airbnb market using a dataset of ~49,000 listings. 
The goal is to clean "dirty" real-world data, identify pricing trends, and find potential investment opportunities for a real estate fund.

**Business Questions:**
1. Which neighbourhoods are the most expensive/cheapest?
2. How does the room type affect the price?
3. Are there any pricing anomalies or outliers?

## 🛠️ Tools & Technologies
*   **Python** (Pandas, NumPy)
*   **Data Visualization** (Matplotlib, Seaborn)
*   **Jupyter Notebook**

## 🧹 Key Data Cleaning Steps
Real-world data often requires significant preparation. Key steps taken:
*   **Handling Missing Values:** Imputed missing values in `reviews_per_month` with 0 and handled missing names.
*   **Date Conversion:** Converted `last_review` to datetime objects.
*   **Outlier Removal:** 
    *   Removed listings with Price = $0.
    *   Applied **Winsorization (99th percentile)** to cap extreme prices at $799 to avoid skewed analysis.
    *   Capped `minimum_nights` at 30 days to focus on short-term rentals.

## 📊 Key Insights
*   **Price Distribution:** The majority of listings are under $200/night. The top 1% of luxury listings (>$800) were capped for better visualization.
*   **Location:** Manhattan is the most expensive borough, while Brooklyn offers a wider range of affordable options.
*   **Availability:** Listings with high availability tend to have lower prices/more reviews.

## 📈 Visualizations

*Check out the interactive Dashboard on Tableau Public:* []

---
*Author: Hanna Kovalenko*
