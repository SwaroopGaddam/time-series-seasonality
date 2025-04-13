# 📈 Time Series Seasonality

This project focuses on analyzing and extracting **seasonality patterns** from monthly sales data using time series decomposition techniques. It includes data trimming, exploratory visualizations, and saving the seasonal components for business insights and forecasting use.

---

## 🔁 Project Steps

### 1. Input Data
- Load monthly (or) quartertly sales data into a pandas DataFrame.
- Convert the `Period` column to a datetime format and set it as the index for time series operations.

### 2. Trim the Dataset
- Use `start_point` and `end_point` to remove rows from the beginning or end if needed.

### 3. Visualization & Analysis
- Plot line charts to observe sales trends.
- Add a 3-month rolling mean to smooth out fluctuations and compare it with original sales plot.
- Visualize distributions using boxplot.

### 4. Seasonality Calculation
- Use `seasonal_decompose` (additive model, period = 12 for monthly data) to extract:
  - **Trend**
  - **Seasonal component**
  - **Residuals**

### 5. Saving Output
- Convert the seasonal component (a pandas Series) into a DataFrame.
- Save it as a CSV file using `to_csv()`.

---

## 🛠️ Libraries Used

- `pandas`
- `matplotlib`
- `seaborn`
- `statsmodels`

---

## 📁 Output

- `seasonality_output.csv`: Contains the extracted seasonal values for each time period.

---

## ✅ Use Cases

- Understanding recurring patterns in sales
- Preparing data for time series forecasting models
- Supporting strategic planning and business decisions

---

Feel free to explore the notebook and modify the code for your own time series datasets!
