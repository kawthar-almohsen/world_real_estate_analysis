# world_real_estate_analysis
---

# 🏡 World Real Estate Data Analysis

## 📌 Project Overview

This project analyzes a dataset of **147,000+ real estate listings** from around the world. Using **Python, Pandas, and Jupyter Notebook**, we explored global property markets to answer key questions about:

* **Pricing** – Where are properties the most expensive or affordable?
* **Demand & Supply** – Which markets are the most active?
* **Investment Opportunities** – Where do buyers get the best value for money?
* **Quality & Features** – How do building age and amenities affect property values?

Our goal was to transform raw data into **actionable insights** for investors, developers, and agencies.

---

## 📊 Dataset & Data Dictionary

The dataset contained real estate listings with the following main columns:

| Column                       | Description                   | How We Used It                          |
| ---------------------------- | ----------------------------- | --------------------------------------- |
| `country`                    | Country of property           | Grouping for comparisons                |
| `location`                   | City/region                   | Used to fill missing values             |
| `title`                      | Property title/description    | Extracted missing country/location info |
| `price_in_USD`               | Property price (USD)          | Key measure of affordability/luxury     |
| `size_m2`                    | Property size (m²)            | Used for price-per-m²                   |
| `apartment_bedrooms`         | Number of bedrooms            | Median imputation for missing values    |
| `apartment_bathrooms`        | Number of bathrooms           | Median imputation for missing values    |
| `construction_year_fixed`    | Corrected construction year   | Derived for analysis                    |
| `building_age`               | 2025 - construction year      | Used in age vs price analysis           |
| `price_per_m2`               | Price / size                  | Fair market comparison                  |
| `floor_number`               | Apartment floor (if present)  | For floor vs price analysis             |
| `url`                        | Listing link                  | Dropped after cleaning                  |

---

## 🧹 Data Cleaning

Steps we took to prepare the dataset:

* Filled missing bedrooms/bathrooms using **median per location**.
* Corrected invalid construction years (<1000).
* Created new columns: `building_age`, `price_per_m2`.
* Dropped irrelevant columns like `url`.
* Removed `"m²"` text from size to keep numeric values.

---

## 📈 Key Analysis Questions

We answered the following questions using Pandas groupby, filtering, and visualizations:

1. **Which countries have the most real estate listings?**
2. **What is the average and median property price per country?**
3. **What is the average price per square meter by country?**
4. **Which countries have the highest share of luxury properties (\$1M+)?**
5. **Which countries have the most newly built homes (2020+)?**
6. **How does building age affect property prices?**

---

## 📊 Visualizations

We created different types of charts to explain insights clearly:

* **Bar charts** → Rankings (e.g., top 10 countries by price).
* **Scatter plots** → Correlation (building age vs price).
* **Pie charts** → Market share (luxury properties).
* **Horizontal bars** → Value-for-money .

---

## 💡 Key Findings

* **Italy** dominates luxury markets with the highest prices.
* **Montenegro and Latvia** stand out as affordable markets.
* **Turkey** has the highest number of listings → most active market.
* **Newly built homes** (2020+) are concentrated in certain countries, showing modern housing supply.
* **Building age** strongly affects prices, but **prime location** can make older properties expensive.
---

## 🚀 Business Benefits

* **Agencies** → Can focus marketing on active, high-liquidity countries.
* **Investors** → Can identify both luxury and affordable growth markets.
* **Developers** → Can target regions with demand for new modern housing.

---

## 🛠️ Tools Used

* **Python**
* **Pandas & NumPy** – Data cleaning & transformation
* **Matplotlib & Seaborn** – Visualizations
* **Jupyter Notebook** – Analysis environment
* **PowerPoint** – Presentation of results

---

## 👩‍💻 Team Members

* Fatima Qasim
* Kawthar Al Mohsen
* Hasan Al Hashemi


---

## ✅ Conclusion

This project shows how **data-driven analysis** can uncover market patterns and provide actionable insights in real estate. By combining Python data analysis with clear visualization and business framing, we created a foundation for smarter investment and development strategies worldwide.

---

⚡ Do you also want me to add a **Getting Started section with setup commands** (like `pip install pandas matplotlib seaborn` and `jupyter notebook`) so your instructor can run your notebooks easily?
