# 🚀 Real-Time Data Processing System for Weather Monitoring with Rollups and Aggregates

### 📜 Objective
Develop a real-time data processing system to monitor weather conditions and provide summarized insights using rollups and aggregates. The system will utilize data from the OpenWeatherMap API (https://openweathermap.org/).

---

## 📊 Data Source
The system will continuously retrieve weather data from the OpenWeatherMap API. You will need to sign up for a free API key to access the data. The API provides various weather parameters, and for this project, we will focus on:
- **main**: Main weather condition (e.g., Rain, Snow, Clear)
- **temp**: Current temperature in Celsius
- **feels_like**: Perceived temperature in Celsius
- **dt**: Time of the data update (Unix timestamp)

---

## 🔄 Processing and Analysis
- The system should continuously call the OpenWeatherMap API at a configurable interval (e.g., every 5 minutes) to retrieve real-time weather data for the metros in India (Delhi, Mumbai, Chennai, Bangalore, Kolkata, Hyderabad).
  
- For each received weather update:
  - Convert temperature values from Kelvin to Celsius (you can also use user preference).

---

## 📈 Rollups and Aggregates

### 1. Daily Weather Summary:
- Roll up the weather data for each day.
- Calculate daily aggregates for:
  - Average temperature
  - Maximum temperature
  - Minimum temperature
  - Dominant weather condition (explain the reasoning).

- Store the daily summaries in a database or persistent storage for further analysis.

### 2. Alerting Thresholds:
- Define user-configurable thresholds for temperature or specific weather conditions (e.g., alert if temperature exceeds 35 degrees Celsius for two consecutive updates).
  
- Continuously track the latest weather data and compare it with the thresholds.
  
- If a threshold is breached, trigger an alert for the current weather conditions. Alerts could be displayed on the console or sent through an email notification system (implementation details left open-ended).

### 3. Implement Visualizations:
- To display daily weather summaries, historical trends, and triggered alerts.

---

## ✅ Test Cases

### 1. System Setup:
- Verify that the system starts successfully and connects to the OpenWeatherMap API using a valid API key.

### 2. Data Retrieval:
- Simulate API calls at configurable intervals.
- Ensure the system retrieves weather data for the specified locations and parses the response correctly.

### 3. Temperature Conversion:
- Test conversion of temperature values from Kelvin to Celsius (or Fahrenheit) based on user preference.

### 4. Daily Weather Summary:
- Simulate a sequence of weather updates for several days.
- Verify that daily summaries are calculated correctly, including average, maximum, minimum temperatures, and dominant weather condition.

### 5. Alerting Thresholds:
- Define and configure user thresholds for temperature or weather conditions.
- Simulate weather data exceeding or breaching the thresholds.
- Verify that alerts are triggered only when a threshold is violated.

---

## 🎁 Bonus Features
- Extend the system to support additional weather parameters from the OpenWeatherMap API (e.g., humidity, wind speed) and incorporate them into rollups/aggregates.
- Explore functionalities like weather forecast retrieval and generating summaries based on predicted conditions.

---

## 🛠️ How to Use This Application

### 1. **Clone the Repository**  and Run in Live Server 
```bash
git clone https://github.com/ashirbadpanda/Application-2-Real-Time-Data-Processing-System-for-Weather-Monitoring-with-Rollups-and-Aggregates

