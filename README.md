# COVID-19 and World Happiness Data Analysis 📊🌍

This project analyzes the relationship between COVID-19 pandemic data and the World Happiness Index using Python. It combines real-world datasets to perform data cleaning, merging, visualization, and statistical correlation analysis.

## 📁 Datasets Used

1. **COVID-19 Dataset**: Confirmed cases, deaths, and recoveries per country.
2. **World Happiness Report**: Includes GDP per capita, social support, healthy life expectancy, and other happiness-related indicators.

> **Note**: Make sure both datasets are downloaded and correctly placed in your working directory before running the script.

## 🛠️ Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- plotly (optional for interactive plots)

## 📌 Steps Performed

### 1. Data Loading
- Imported and loaded the two datasets using `pandas.read_csv`.

### 2. Data Cleaning
- Checked for missing values and removed any incomplete records using `dropna()`.

### 3. Data Transformation
- Aggregated the COVID-19 dataset by country.
- Renamed and standardized country names for merging compatibility.
- Merged both datasets on the "Country" column.

### 4. Exploratory Data Analysis (EDA)
- Generated correlation heatmaps using `seaborn.heatmap`.
- Created scatter plots to study relationships between:
  - **GDP per capita vs Confirmed Cases**
  - **Healthy Life Expectancy vs Deaths**
  - **Social Support vs Recoveries**

### 5. Insights
- **GDP vs Confirmed**: Moderate positive correlation.
- **Life Expectancy vs Deaths**: Positive correlation; healthier countries report more deaths (possibly due to better reporting).
- **Social Support vs Recovery**: Mild correlation; indicates societal factors may affect health outcomes.

## 📉 Visualizations

| Graph | Description |
|-------|-------------|
| Heatmap | Shows correlation between happiness and COVID indicators |
| Scatter Plot 1 | GDP per capita vs Confirmed COVID cases |
| Scatter Plot 2 | Life Expectancy vs COVID Deaths |
| Scatter Plot 3 | Social Support vs Recoveries |

## 📈 Sample Output

```python
Correlation between GDP and Confirmed Cases: 0.47
Correlation between Life Expectancy and Deaths: 0.45
Correlation between Social Support and Recoveries: 0.33
