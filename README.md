# 📉 Unemployment Analysis in India (Data Science Project)

This project analyzes unemployment trends in India using real-world datasets.
It includes data cleaning, visualization, trend analysis, and regional unemployment comparison using Python.

This project is part of the **Data Science Internship Task**.

---

## 📂 Project Overview

Unemployment is a major economic indicator, and analyzing its patterns helps understand:

* Trends over time
* Regional variations
* Correlations between economic factors
* Overall unemployment conditions in the country

This project uses **two datasets** to study unemployment in India up to November 2020.

---

## 📁 Datasets Used

The project uses two CSV files:

1. **Unemployment in India.csv**
2. **Unemployment_Rate_upto_11_2020.csv**

Both datasets include:

* Date
* Region
* Estimated Unemployment Rate (%)
* Estimated Employed
* Estimated Labour Participation Rate (%)

Dataset cleaning includes:

* Removing spaces from column names
* Fixing and converting the date column
* Handling missing values

---

## 🛠️ Tools & Libraries

* **Python**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Google Colab**

---

## 📊 Visualizations & Analysis

### 📈 1. Unemployment Trend Over Time

A line plot shows how unemployment rate changes with time.

```python
plt.plot(df2[date_column], df2["Estimated Unemployment Rate (%)"])
```

This reveals rising and falling patterns of unemployment.

---

### 📦 2. Region-wise Unemployment Comparison

A boxplot highlights how unemployment varies across regions in India.

```python
sns.boxplot(data=df2, x="Region", y="Estimated Unemployment Rate (%)")
```

---

### 🔥 3. Correlation Heatmap

Shows relationships between numeric indicators such as unemployment rate, labor participation, etc.

```python
sns.heatmap(numeric_data.corr(), annot=True, cmap="coolwarm")
```

---

### 📊 4. Average Unemployment by Region

A bar chart displaying the average unemployment rate for each region.

```python
region_avg.plot(kind="bar")
```

This helps identify the most and least affected regions.

---

## ✔️ Key Findings

* Clear trends in unemployment across months
* Strong differences in unemployment across regions
* Useful correlations between economic indicators
* Insights useful for economic research & policymaking

---

## 🚀 How to Run

1. Clone the repository:

```
git clone https://github.com/your-username/your-repository.git
```

2. Install required libraries:

```
pip install pandas matplotlib seaborn
```

3. Upload datasets and run the script in **Google Colab** or **Jupyter Notebook**.

---

## 📌 Future Improvements

* Add forecasting using ARIMA or Prophet
* Build a dashboard using Power BI or Tableau
* Deploy visualization using Streamlit

---

## 🤝 Contributing

Contributions and suggestions are welcome!

---

## ⭐ Support

If you found this project helpful, consider giving it a **star ⭐ on GitHub**.

---

## 📝 License

This project is open-source and free to use.

---
