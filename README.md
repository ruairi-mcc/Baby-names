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
