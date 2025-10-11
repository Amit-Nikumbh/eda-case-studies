# 🛫 Airlines Flights EDA

Exploratory Data Analysis (EDA) of **Indian domestic flight data** covering ticket prices, travel routes, booking patterns, and airline performance.
This analysis explores how factors like **source/destination, flight class, airline, and booking window** influence fares and travel trends.

---

## 📦 Dataset

**Source:** [Kaggle – Airlines Flights Data](https://www.kaggle.com/datasets/rohitgrewal/airlines-flights-data)
**Records:** 300,153 rows
**Features:** 11 columns including `airline`, `source_city`, `destination_city`, `class`, `duration`, `days_left`, and `price`.

---

## 🎯 Objectives

* Understand flight data structure and distribution
* Identify pricing patterns across routes and classes
* Analyze airline-level offerings (Economy vs Business)
* Study booking behavior (planned vs unplanned)
* Create storytelling visuals and actionable insights

---

## 🧰 Tools & Libraries

| Category      | Tools Used              |
| ------------- | ----------------------- |
| Data Handling | pandas, numpy           |
| Visualization | matplotlib, seaborn     |
| Statistics    | scipy.stats (trim_mean) |
| Notebook      | Jupyter Notebook        |

---

## 📊 Analysis Workflow

### 1. **Data Overview**

* No missing or duplicate records
* Mixed data types: categorical (routes, airlines), numeric (price, duration)
* Converted categorical columns to `category` dtype for optimization

### 2. **Univariate Analysis**

* **Numerical:** `price`, `duration`, `days_left`

  * Right-skewed distributions; few long-haul/premium outliers
* **Categorical:** `airline`, `class`, `stops`, `departure_time`, `arrival_time`

  * Vistara & Air India dominate (~69%)
  * 80% of flights have 1 stop; majority are Economy class

### 3. **Bivariate & Multivariate Analysis**

* **Correlation heatmap** between numeric features
* **Route-wise price heatmaps** for Economy & Business
* **Crosstab** for airline vs class proportions
* **Booking window vs price** impact visualization

### 4. **Feature Engineering**

* `price_per_hour` – normalized fare
* `is_business` – binary indicator
* `booking_type` – categorized into *Well-planned*, *Planned*, *Unplanned*

---

## 💡 Key Insights

### ✈️ Route & Class

* **Kolkata routes** (esp. Kolkata–Chennai, Kolkata–Hyderabad) are premium priced
* **Mumbai–Delhi** and **Mumbai–Hyderabad** are most economical
* Business fares are **6–8× higher** than Economy on the same route

### 🕐 Booking Behavior

| Booking Type            | Economy (₹) | Business (₹) | Difference          |
| ----------------------- | ----------- | ------------ | ------------------- |
| Well-planned (>30 days) | 4,919       | 51,649       | ↓ Up to 60% cheaper |
| Unplanned (≤2 days)     | 14,226      | 61,206       |                     |

* Early booking drastically reduces fares, especially for Economy class.

### 🏙️ Airlines

* **Air India & Vistara** – only ones offering both classes
* **AirAsia** – lowest average Economy fare
* **Vistara** – highest Business class pricing

---

## 📈 Visual Highlights

* Histograms & Boxplots for distribution understanding
* Heatmaps for route-based pricing
* Barplots for airline & booking class comparison
* Line plots for time-based fare variations

All visuals are exported under the `visuals/` folder.

---

## 🧩 Folder Structure

```
Airlines-EDA/
│
├── airlines_eda.ipynb      # Main analysis notebook
├── data/                   # Dataset or Kaggle link reference
├── visuals/                # Charts & exported plots
└── README.md               # Project documentation
```

---

## 🏁 Conclusion

* Flight pricing strongly depends on **route, class, and booking timing**.
* **Kolkata routes** remain the most expensive across both classes.
* **Mumbai and Delhi** continue to be the most affordable hubs.
* Early planning and route optimization can lead to **significant savings**.

---

## 🚀 Next Steps

* Add time-series trend analysis (if timestamp available)
* Predict flight prices using regression models
* Extend to multi-airline comparison dashboard using Plotly/Dash

---
