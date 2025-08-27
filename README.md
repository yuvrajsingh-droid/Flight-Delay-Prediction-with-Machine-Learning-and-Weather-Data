# ✈️ Flight Delay Prediction with Machine Learning

## 📌 Overview
Flight delays are a common problem in aviation, impacting airlines, airports, and passengers.  
This project leverages **flight schedule data and weather information** to predict whether a flight will be delayed at departure.  

The dataset (`M1_final.csv`) contains detailed flight records combined with weather data, and the notebook (`GrpP2flightdelay.ipynb`) provides the full workflow from preprocessing to prediction.

---

## 📊 Dataset
- **Rows:** 28,820  
- **Columns:** 23  
- **Target Variable:** `DEP_DELAY` (numeric: minutes of delay, negative = early departure, positive = delayed departure)  

### Features:
- Flight Details:  
  - `MONTH`, `DAY_OF_MONTH`, `DAY_OF_WEEK`  
  - `OP_UNIQUE_CARRIER`, `TAIL_NUM`, `DEST`  
  - `DEP_DELAY`, `CRS_ELAPSED_TIME`, `DISTANCE`  

- Timing Features:  
  - `CRS_DEP_M`, `DEP_TIME_M`, `CRS_ARR_M`, `sch_dep`, `sch_arr`, `TAXI_OUT`  

- Weather Conditions:  
  - `Temperature`, `Dew Point`, `Humidity`, `Wind`, `Wind Speed`, `Wind Gust`, `Pressure`, `Condition`  

---

## ⚙️ Project Workflow
1. **Data Cleaning**  
   - Handle missing values (`Wind`)  
   - Convert time features into meaningful categories  
   - Encode categorical variables (airlines, destinations, weather conditions)  

2. **EDA (Exploratory Data Analysis)**  
   - Analyze distribution of delays  
   - Relationship between weather & flight delays  
   - Peak times and routes for delays  

3. **Modeling Approaches**  
   - Regression (predict delay in minutes)  
   - Classification (Delayed vs On-Time flights)  
   - Models: Logistic Regression, Random Forest, Gradient Boosting, XGBoost  

4. **Evaluation Metrics**  
   - Accuracy, Precision, Recall, F1-score  
   - ROC-AUC for classification  
   - RMSE/MAE for regression  

---


