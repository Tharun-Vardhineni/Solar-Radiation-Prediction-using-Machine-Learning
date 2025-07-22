# ☀️ Solar Radiation Prediction using Machine Learning

## 📘 About the Project

This project focuses on analyzing and predicting **solar radiation** using historical weather and solar data collected in Hawaii. The goal is to better understand solar energy trends and build predictive models using **machine learning**, particularly **Random Forest** algorithms.

Using rich features derived from timestamps (like hour, day of year, and month), we analyze solar behavior over time and train models to predict solar radiation. This kind of analysis can support sustainable energy planning, smart grid optimization, and solar farm management.

---

## ❓ Problem Statement

Solar radiation fluctuates based on time, weather, and seasonal patterns. Accurately predicting solar output is crucial for:

* Energy demand forecasting
* Optimizing solar panel usage
* Scheduling energy storage systems

The key challenge is to build a model that can predict solar radiation using various features like time, temperature, and location-derived data.

---

## 🎯 Objectives

* Load and preprocess the **SolarPrediction** dataset
* Extract and engineer features based on time (e.g., month, hour, day of year)
* Visualize radiation trends across dates
* Handle and check for missing data
* Train a **Random Forest Regressor** to predict solar radiation
* Evaluate model performance using metrics like RMSE and R²

---

## 🛠️ Project Workflow

### 1. **Data Loading & Cleaning**

* Loaded the `SolarPrediction.csv` dataset
* Sorted the data based on UNIX timestamps
* Checked for missing values using visual tools (e.g., seaborn heatmap)
* Cleaned up and prepared timestamps using Python’s `datetime` and `pytz` libraries

### 2. **Feature Engineering**

* Converted UNIX time to localized datetime using Pacific/Honolulu timezone
* Extracted time-based features:

  * `Hour`, `Month`, `DayOfYear`, `WeekOfYear`, etc.
* Calculated **total daytime hours** based on sunrise and sunset times

### 3. **Exploratory Data Analysis (EDA)**

* Plotted **Radiation over time**
* Added mean radiation trendlines to observe fluctuation patterns
* Visualized other time-based trends for pattern identification

### 4. **Modeling**

* Trained a **Random Forest Regressor** on the cleaned dataset
* Selected relevant features for training (not fully shown in the preview)
* Evaluated model performance using common regression metrics

---

## 🧰 Tools & Libraries Used

* **Python**
* **Pandas, NumPy** – for data manipulation
* **Matplotlib, Seaborn, Plotly** – for visualization
* **Scikit-learn** – for building and evaluating machine learning models
* **Datetime, Pytz** – for time-related feature extraction

---

## 📈 Key Insights

* Solar radiation follows daily and seasonal patterns, with noticeable dips and spikes
* Time-based features significantly impact model accuracy
* Random Forest performed well in modeling nonlinear behavior in solar output

---

## 🚀 Future Enhancements

* Include weather features like humidity, temperature, wind speed, etc. if available
* Try deep learning models (e.g., LSTM for time series forecasting)
* Deploy the model using a web app (e.g., Streamlit or Flask)
* Add real-time data integration (e.g., via weather APIs)

---
