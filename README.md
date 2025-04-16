# 📊 Baby Name Popularity in Ireland

This project is an interactive data visualization web application built with **Dash** and **Plotly**, exploring trends in Irish baby names from 1964 to 2023.

It includes:
- Popularity over time comparisons
- Seasonal trend decomposition
- Most popular names by year
- Unique name counts and fada (accented) name usage

---

## 📁 Dataset

Two CSV files are used:
- `Boys names.csv`
- `Girls names.csv`

These are sourced from the [CSO Ireland baby names statistics](https://www.cso.ie).

Each dataset contains annual name usage data including:
- Year
- Name
- Gender
- Count (`VALUE`)
- Additional metadata

---

## 📦 Dependencies

To run this app, ensure you have the following Python libraries installed:

```bash
pip install pandas numpy matplotlib statsmodels scikit-learn plotly dash seaborn
```

## 🧠 Features & Visualizations

### 🔹 1. Name Popularity Over Time
Compare multiple baby names across years, filtered by gender. Interactive line charts display trends clearly.

### 🔹 2. Trend & Seasonality Analysis
Applies seasonal decomposition using `statsmodels` to break down the time series data into:
- 📈 **Trend**: Underlying direction
- 🔁 **Seasonal**: Repeating patterns
- 🔹 **Residual**: Random noise

### 🔹 3. Top 10 Names by Year
Select any year to see the top 10 most popular boy and girl names displayed side-by-side in bar charts.

### 🔹 4. Distribution Analysis
Explore the makeup of name characteristics:
- 🔢 **Name length distribution** across all unique names
- 🆔 **Unique name counts** by gender
- 🇮🇪 **Fada (accented) name usage** over time (e.g., á, é, í, ó, ú)

---

## 📊 Sample Insights

- **Unique Names**:
  - 👦 **Boys**: 2,662
  - 👧 **Girls**: 3,604

- **Accented (Fada) Names Over Time**:
  - 📉 1964–2017: Near-zero usage
  - 📈 2018–2023: Rapid increase
    - 2018: 3,095 babies with fada names
    - 2023: 4,120 babies with fada names

These insights show a clear cultural shift and diversification in Irish baby naming practices.
