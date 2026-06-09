# Egypt Used Cars Market Data Analytics Project

## 📌 Project Overview
This is an **End-to-End Data Analytics project** built with Python to simulate, clean, analyze, and visualize used car market trends in Egypt. 

The project demonstrates a complete data professional workflow: overcoming data acquisition constraints, cleaning unstructured text data, applying business-driven missing value imputation, conducting Exploratory Data Analysis (EDA), and creating professional data visualizations.

---

## 🏗️ Data Architecture & Lifecycle

### 1. Data Simulation & Acquisition
* **Challenge:** Direct web scraping from local automotive platforms faced robust anti-scraping policies (e.g., HTTP 403 Forbidden errors due to automated environments).
* **Solution:** Developed a programmatic data generation script that simulates a highly realistic dataset of **250 used car listings** matching real-world Egyptian market dynamics, brand distributions, and pricing tiers (including Hyundai, Kia, Toyota, Chevrolet, and Fiat).
* **Data Anomaly Injection:** Purposefully injected missing values (`NaN` in prices) and extreme outliers (unusually high mileages) to recreate authentic, messy real-world data environments.

### 2. Data Cleaning & Preprocessing
* Removed regional currency strings (`EGP`) and localized thousands separators (commas) using regular expressions.
* Handled missing price entries utilizing a **Groupby Imputation Strategy** (replacing missing prices with the calculated mean price of that specific car's Brand and Model) to preserve dataset integrity and business logic.
* Converted cleaned features into optimized numeric data types (`int` and `float`) for advanced computational analytics.

### 3. Exploratory Data Analysis (EDA) & Insights
The dataset was aggregated to extract high-value business insights regarding the Egyptian automotive sector:
* **Market Share:** Identified the most frequently listed automotive brands.
* **Pricing Tiers:** Analyzed the average valuation of each brand, highlighting premium segments (e.g., Kia and Hyundai) versus budget-friendly segments (e.g., Fiat).
* **Vehicle Utilization:** Evaluated the highest mileage models to identify the most heavily utilized vehicles in the market.

### 4. Advanced Data Visualization
Generated publication-quality dual-faceted statistical plots using `Seaborn` and `Matplotlib`:
* **Bar Plot:** Displays a clear ranking of average car prices sorted by brand.
* **Multi-Dimensional Scatter Plot:** Illustrates the correlation between manufacturing year and listing price, dynamically colored by vehicle condition (Nearly New vs. Used) and sized according to overall mileage (KM).

---

## 🛠️ Technologies Used
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Google Colab / Jupyter Notebooks

---

## 🚀 How to Run the Project
1. Clone this repository:
   ```bash
   git clone [https://github.com/abdallasaad35/egypt-used-cars-analysis.git](https://github.com/abdallasaad35/egypt-used-cars-analysis.git)
