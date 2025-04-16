# 📊 Baby Name Popularity in Ireland

This project is an interactive data visualization web application built with **Dash** and **Plotly**, exploring trends in Irish baby names from 1964 to 2023.

It includes:
- Popularity over time comparisons
- Seasonal trend decomposition
- Most popular names by year
- Unique name counts and fada (accented) name usage

  This data shows that  baby names in Ireland have steadily moved from the same traditional names in the 1960s, 70s and 80s to a more diverse selection of names. The number of unique names in 1964 was 268 which explodes to 989 by 2023 highilighting a growing cultural diversity but also a move away from the samaller pool of *"Christian"* names. 

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
      
  ## A follow up inquiry with the CSO confimed that this is an artefact of the system that was used to input data...

   *"From 01 January 2018 the CSO has captured the síneadh fada and other diacritics for the first time. This marks the beginning of new series of data. The inclusion of the síneadh fada and other diacritics has an impact     in the order of the popularity of some forenames. For example Sean (without the síneadh fada) has always been in the top 100 most popular names for boys. Seán with the síneadh fada is now included in the 2018 data          onwards and both spellings are treated as 2 separate names and thus it fell out of the top 100 in 2019. At the beginning of the collection process, names had to be manually inputted on a database from paper records.        This was a labour-intensive task and a decision was taken in 1998 to input names without síneadh fadas. When data became digitally available it was decided to continue as before, as any change would result in a break in    the series."*
