# 🌦️ Analysis of Recent Weather Conditions in Almaty

## 📌 Project Overview
This project analyzes recent weather patterns in Almaty, Kazakhstan, using web scraping, data processing, augmentation, and visualization techniques. A supervised machine learning model is developed to predict future weather conditions. This study aims to provide insights into climatic trends, aiding in better decision-making for local industries and communities.

## 👨‍💻 Group Members
- **Mansurkhan Aknur** 
- **Iliyas Aruzhan** 
- **Zhurymbay Akbike**

## 🛠 Project Workflow
### 📥 1. Data Collection & Scraping
- Data is scraped from 🌍 [World Weather Online](https://www.worldweatheronline.com/).
- The dataset contains weather information for today and the next 15 days.
- The collected data is stored in `weather_info.csv` with 📊 360 rows and 10 columns.

### 🧹 2. Data Cleaning
- ✅ Checked for missing values (none found).
- ✅ Checked for duplicate records (none found).
- ✅ Ensured correct data types.

### 📊 3. Data Augmentation
- Calculated new weather-related metrics:
  - 🌡️ **Temperature Range** = Temperature - Feels Like Temperature
  - 💨 **Wind Chill** = 13.12 + 0.6215T - 11.37V^0.16 + 0.3965TV^0.16
  - ☀️ **Heat Index** = −8.784695 + 1.61139411T + 2.338549H - 0.14611605TH
  - 🌧️ **Rain Intensity** = (Rain % × Rain (mm)) / 100
  - 🌬️ **Wind Gust Difference** = Gust (km/h) − Wind (km/h)

### 📈 4. Data Visualization
- Created charts and graphs to analyze 📉 weather trends.

### 🤖 5. Machine Learning Model
- Trained a **supervised ML model** to predict future weather conditions.
- The prediction model dynamically updates as new data is scraped.

## 🔧 Technologies Used
- 🕵️ **Web Scraping**: `BeautifulSoup`, `requests`
- 📊 **Data Processing & Analysis**: `Pandas`, `NumPy`
- 📉 **Visualization**: `Matplotlib`, `Seaborn`
- 🤖 **Machine Learning**: `Scikit-learn`
