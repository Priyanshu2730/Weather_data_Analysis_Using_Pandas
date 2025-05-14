# 🌦️ Weather Data Analysis Using Pandas

This project is an exploratory data analysis (EDA) of a weather dataset using **Pandas**. The aim is to derive meaningful insights and practice data wrangling by solving real-world data questions. It involves data cleaning, transformation, statistical analysis, and logical filtering.

## 📌 Objective

To analyze a weather dataset and answer a set of 15 diverse questions using **Python** and **Pandas**, covering:

- Data exploration and cleaning
- Statistical analysis (mean, standard deviation, variance)
- Conditional filtering
- Grouping and aggregation
- String-based condition matching

## 📂 Dataset

The dataset includes weather-related features like:

- Date/Time
- Temperature
- Wind Speed
- Weather Condition
- Visibility
- Relative Humidity
- Pressure

## ✅ Key Questions Solved

1. Unique Wind Speed values
2. Count of records where weather is exactly 'Clear'
3. Count of records with wind speed of 4 km/h
4. Detection of null values
5. Renaming the 'Weather' column to 'Weather Condition'
6. Mean visibility
7. Standard deviation of pressure
8. Variance of relative humidity
9. All records where snow was recorded
10. Records with wind speed > 24 and visibility = 25
11. Mean of all columns grouped by weather condition
12. Minimum & maximum of all columns grouped by weather condition
13. All records where weather condition is 'Fog'
14. All instances where weather is 'Clear' or visibility > 40
15. All instances where:
    - Weather is 'Clear' and humidity > 50  
    - OR visibility > 40

## 🔍 Sample Code Snippets


# Q2. Number of times weather is exactly Clear
WD[WD['Weather'] == 'Clear'].shape[0]

# Q4. Check for null values
WD.isnull().sum()

# Q11. Mean of each column grouped by weather condition
WD.groupby('Weather Condition').mean(numeric_only=True)

## 📊 Insights
Clear weather was observed multiple times, but Fog and Snow conditions were less frequent.

Wind Speed of 4 km/h occurred rarely, indicating most of the time, wind speed was either higher or lower.

Visibility had a significant impact — many days with high visibility (>40) also had clear or partly cloudy weather.

Some combinations like high wind speed with low visibility are rare and could indicate unusual weather conditions.

The dataset was clean overall, with very few or no null values.

🚀 Tools Used
  Python

  Pandas

  Jupyter Notebook / Google Colab

📁 How to Run
Clone this repository.

Install dependencies:
    pip install pandas
Run the notebook in any Jupyter environment.




