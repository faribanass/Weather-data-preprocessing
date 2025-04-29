# 🌦️ Weather Data Analysis Project

This repository contains a basic data exploration project using a global weather dataset. The dataset includes weather-related observations from countries across the world, with features such as temperature, wind speed, air quality, humidity, and more.

## 📁 Dataset

- **File Name**: `GlobalWeatherRepository.csv`
- **Size**: 54,568 rows × 41 columns
- **Columns Include**:
  - City, Location, Latitude/Longitude
  - Temperature in Celsius/Fahrenheit
  - Weather condition
  - Wind speed, humidity, air pressure
  - Sunrise, sunset, moon phase, air quality indices, etc.


The dataset used in this project is from Kaggle and is not included in this repository due to license restrictions.

You can download it manually from the link below (Kaggle account required):

🔗 [Download Global Weather Dataset from Kaggle](https://www.kaggle.com/datasets/henryshan/globalweatherrepository)

Once downloaded, rename the file (if needed) to `GlobalWeatherRepository.csv` and place it in the project root directory.

## 📊 What’s Covered

The notebook performs the following tasks:

1. **Loading and inspecting the data**
   - `df.head()`, `df.shape`, `df.columns`, `df.dtypes`
2. **Missing values check**
   - `df.isnull().sum()`
3. **Exploratory Data Analysis (EDA)**:
   - Unique values and counts of `condition_text`, `wind_kph`, etc.
   - Filtering for specific conditions like `'Clear'`, `'Snow'`
   - Renaming columns (`condition_text` → `weather_condition`)
4. **Descriptive Statistics**:
   - Mean visibility
   - Standard deviation of pressure
   - Variance of humidity
5. **Condition-based Filtering**:
   - All entries with snow in weather conditions
   - Locations with wind speed exactly 4 kph

## 📌 Sample Insights

- Most common weather condition: *Partly cloudy*
- Number of unique `wind_kph` values: 174
- Entries with `wind_kph == 4`: 974 rows
- Entries with `condition_text == "Clear"`: 2273 rows
- Heavy snow was recorded in multiple countries including Finland, Afghanistan, and Ukraine.

## 🛠️ Tools Used

- Python
- Pandas
- Jupyter Notebook

## 🚀 How to Run

```bash
pip install pandas
```

Run the code in a Jupyter Notebook or any Python environment after downloading the dataset.

## 📌 Author

This project was created as a learning exercise to practice basic data analysis using the Pandas library.
