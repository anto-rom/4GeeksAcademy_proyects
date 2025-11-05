# 🏡 Exploratory Data Analysis of Airbnb Listings

## 📄 Project Overview

This project performs an **Exploratory Data Analysis (EDA)** on an Airbnb dataset to uncover insights about pricing patterns, availability, reviews, and property characteristics. The objective is purely analytical — **no predictive modeling or machine learning** is included.

## 🎯 Objectives

* Understand the structure and quality of the dataset.
* Detect missing values, data types, and potential inconsistencies.
* Explore **numerical** and **categorical** features to identify trends.
* Analyze **distributions**, **outliers**, and **correlations** between key variables.
* Generate clear, interpretable visualizations to support findings.

## 🧩 Dataset Description

The dataset contains information about Airbnb listings, such as:

* **Location features:** neighbourhood, neighbourhood_group, latitude, longitude
* **Property attributes:** room_type, minimum_nights, availability_365
* **Demand indicators:** number_of_reviews, reviews_per_month
* **Price-related attributes:** price

> The raw data was cleaned and formatted before analysis (e.g., removing currency symbols, handling missing values, and correcting data types).

## 🔍 EDA Workflow

1. **Data Import & Inspection**

   * Loaded dataset with `pandas`
   * Checked dimensions, variable types, and basic statistics
   * Identified nulls, duplicates, and inconsistent entries

2. **Data Cleaning**

   * Converted columns to appropriate types
   * Treated missing values and outliers
   * Ensured numerical consistency for price and review metrics

3. **Univariate Analysis**

   * Distribution plots for key numeric variables (e.g., `price`, `minimum_nights`)
   * Frequency counts for categorical variables (`room_type`, `neighbourhood_group`)

4. **Bivariate & Multivariate Analysis**

   * Correlation matrix for numerical variables
   * Pairwise scatterplots and boxplots to explore variable relationships
   * Cross-tab analysis between room types, location, and price

5. **Outlier Detection**

   * Applied IQR method and visualized distributions to detect extreme values

6. **Data Visualization**

   * Used `matplotlib` and `seaborn` for professional visualizations
   * Highlighted trends such as high-price clusters and review density by neighbourhood

## 📊 Key Insights

* Most listings are **entire homes/apartments** with prices below **€250**, but there are significant outliers above **€1000**.
* **Manhattan and Brooklyn** dominate the listing volume, showing distinct pricing tiers.
* Properties with **shorter minimum stays** attract more reviews per month.
* **Availability** varies seasonally, with clear concentration patterns across neighbourhoods.

## 🛠️ Tools & Libraries

* **Python 3.x**
* **pandas** – data manipulation
* **numpy** – numerical operations
* **matplotlib / seaborn** – visualizations
* **scikit-learn (StandardScaler)** – standardization for comparability

## 🧾 File Structure

```
📁 Airbnb_EDA/
├── EDA_AirBnB.ipynb        # Main Jupyter notebook
├── README.md               # Project documentation
└── data/                   # (Optional) source dataset
```

## 🚀 How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/<your_username>/Airbnb_EDA.git
   cd Airbnb_EDA
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:

   ```bash
   jupyter notebook EDA_AirBnB.ipynb
   ```

## 💡 Conclusion

This exploratory analysis provides an overview of Airbnb market dynamics, highlighting geographic and pricing disparities, as well as behavioral insights from host activity and customer reviews. The findings lay the groundwork for future predictive or business-oriented analyses.

---

**Author:** Antonio Romero
**Purpose:** Educational / Exploratory Data Analysis only
**License:** MIT
