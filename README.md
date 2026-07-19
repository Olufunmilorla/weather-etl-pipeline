# weather-etl-pipeline-
A simple ETL pipeline built with Python that extracts real-time weather data from the OpenWeather API, transforms it using Pandas, and loads it into CSV, Excel, and SQLite formats. Includes basic exploratory analysis and visualizations comparing weather across 5 Nigerian cities.
# 🌦️ Week 7: Weather Data ETL Pipeline

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?logo=pandas)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?logo=sqlite)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

A simple **ETL (Extract, Transform, Load)** pipeline built with Python using real-time weather data from the **OpenWeather API**. This project was completed as part of the **AnalystLab Africa Data Analytics Internship (Batch B)  Week 7** to demonstrate API integration, data transformation, storage, and basic exploratory data analysis.

---

## 📌 Project Overview

Organizations collect data from multiple sources before it can be analyzed. This project demonstrates a complete ETL workflow by extracting live weather data from the OpenWeather API, transforming the raw JSON response into a clean and structured dataset, storing the processed data in multiple formats, and generating basic analytical insights through descriptive statistics and visualizations.

---

## 🎯 Objectives

- Extract real-time weather data from an external API.
- Transform raw JSON responses into a structured dataset.
- Clean and validate the data for analysis.
- Store the processed dataset in reusable formats.
- Perform exploratory data analysis and visualization.

---

## 🌍 Data Source

**API:** [OpenWeather API](https://openweathermap.org/api)

### Cities Covered

- Lagos
- Ibadan
- Umuahia
- Jos
- Abuja

### Weather Variables Retrieved

- City Name
- Temperature (°C)
- Humidity (%)
- Weather Condition
- Wind Speed (m/s)
- Date & Time

---

# 🔄 ETL Process

## 1️⃣ Extract

Connected to the OpenWeather API using Python's **requests** library and retrieved real-time weather data for five Nigerian cities.

For improved security, API credentials were stored in a **.env** file and excluded from version control using **.gitignore**, preventing sensitive information from being exposed.

---

## 2️⃣ Transform

The raw JSON responses were transformed into a clean Pandas DataFrame by:

- Selecting relevant weather variables
- Renaming columns for readability
- Converting timestamps to datetime format
- Validating data types
- Checking for missing values
- Removing duplicate records
- Preparing the dataset for analysis

---

## 3️⃣ Load

The processed dataset was exported into multiple formats for future analysis and reporting.

Generated files:

- weather_data.csv
- weather_data.xlsx
- weather_data.db (SQLite)

---

## 📊 Exploratory Data Analysis

Basic descriptive analysis was performed to compare weather conditions across the selected cities.

The analysis included:

- Average Temperature
- Average Humidity
- Average Wind Speed
- Highest Temperature
- Lowest Temperature
- Highest Humidity
- Weather Condition Distribution

## Visualizations were created using Matplotlib to compare:

### Temperature Comparison

![Temperature Comparison](https://drive.google.com/file/d/1ZQvlyle0KpDL5dycSqUBNsBOid1SujZo/view?usp=sharing)

### Humidity Comparison

![Humidity Comparison](https://drive.google.com/file/d/1mqfR5F0bnbtjq2cuhz3jlKO7qo9biZ80/view?usp=sharing)

### Wind Speed Comparison

![Wind Speed Comparison](https://drive.google.com/file/d/1P59K3Hp8B9KPhQqKcVxFvuP9cZzY-8jX/view?usp=sharing)

### Weather Condition Distribution

![Weather Conditions](https://drive.google.com/file/d/1E3metXSQnCT_aJt0LbFmLz-mDTrL9yH4/view?usp=sharing)

  
## 🎥 Project Demo

A short demonstration of the ETL pipeline is available here:
- **Google Drive:** https://drive.google.com/file/d/14K9NUNRQVY41nlM4fTJhZGZRPnp7JNWx/view?usp=sharing

---

## 🔍 Key Findings

- Abuja recorded the highest temperature (**27.07°C**).
- Jos recorded the lowest temperature (**24.82°C**).
- Ibadan had the highest humidity (**87%**).
- Lagos recorded the highest wind speed (**3.55 m/s**).
- Overcast clouds were the most common weather condition, appearing in four of the five cities.
- The average temperature across all cities was **26.09°C**, indicating generally warm weather conditions.

---

## 🛠️ Technologies Used

- Python
- Pandas
- Requests
- python-dotenv
- Matplotlib
- SQLite
- Jupyter Notebook
- OpenWeather API

---

## 📂 Project Structure

```
weather-etl-pipeline/
│
├── Week7-weather-etl.ipynb
├── weather_data.csv
├── weather_data.xlsx
├── weather_data.db
├── README.md
├── requirements.txt
├── .gitignore
└── images/
    ├── temperature_comparison.png
    ├── humidity_comparison.png
    ├── wind_speed_comparison.png
    └── weather_conditions.png
```

---

## ▶️ How to Run

Clone the repository:

```bash
git clone https://github.com/yourusername/weather-etl-pipeline.git
```

Navigate into the project folder:

```bash
cd weather-etl-pipeline
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Create a **.env** file and add your OpenWeather API key:

```text
API_KEY=your_api_key_here
```

Open the notebook and run all cells.

---

## 📚 Learning Outcomes

This project strengthened my understanding of:

- Building ETL pipelines with Python
- Consuming REST APIs
- JSON data processing
- Data transformation using Pandas
- Data quality validation
- Exporting datasets into multiple formats
- Exploratory Data Analysis (EDA)
- Data visualization with Matplotlib

---

## 👨‍💻 Author

**Olufunmilola Ogunmefun**

Aspiring Data Analyst | Python | SQL | Excel | Power BI

Completed as part of the **AnalystLab Africa Data Analytics Internship (Batch B)**.

---

⭐ If you found this project helpful, consider giving the repository a star.
