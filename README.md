# Bird-Migration-Success-Predictor
"A good project name should be clear, descriptive, and reflect the purpose. Since your project predicts bird migration success using environmental and flight-related data"

<img src="https://github.com/rpjinu/Bird-Migration-Success-Predictor/blob/main/bird_image.png">

# 🐦 Bird Migration Pattern Prediction

Welcome to the **Bird Migration Pattern Prediction** project! This project utilizes real-world bird migration data to predict whether a bird's migration will be successful based on environmental and behavioral factors using machine learning classification models. 🌍✨

---

## 📌 Project Overview

Bird migration is a vital phenomenon influenced by various environmental and biological factors. This project aims to:

- Analyze and visualize migratory bird data
- Clean and preprocess the dataset
- Train and evaluate multiple classification models
- Predict migration success (`Migration_Success`)
- Identify key influencing features on successful migration
- Deploy a predictive model for real-time insights

---

## 📁 Dataset Description

The dataset contains a range of features related to bird species, migration patterns, environmental conditions, and tagging metadata.

### 🔑 Key Features Used:

- `Species`
- `Region`
- `Habitat`
- `Weather_Condition`
- `Migration_Reason`
- `Flight_Distance_km`
- `Flight_Duration_hours`
- `Average_Speed_kmph`
- `Temperature_C`
- `Wind_Speed_kmph`
- `Humidity_%`
- `Pressure_hPa`
- `Visibility_km`
- `Nesting_Success`
- `Migration_Start_Month`
- `Migration_End_Month`
- `Rest_Stops`
- `Predator_Sightings`
- `Migrated_in_Flock`
- `Flock_Size`
- `Food_Supply_Level`
- `Migration_Interrupted`
- `Interrupted_Reason`

🎯 **Target Column:** `Migration_Success` (0 = Failed, 1 = Successful)

---

## 🔧 Project Pipeline

### 1. 🧼 Data Cleaning & Preprocessing
- Dropped irrelevant columns such as GPS coordinates, tag details, observer info, etc.
- Handled missing values
- Applied Label Encoding to categorical columns

### 2. 📊 Exploratory Data Analysis (EDA)
- Visualized distributions of important features
- Analyzed `Interrupted_Reason` using count plots with seaborn palettes
- Identified correlations and trends

### 3. 🧠 Model Training & Evaluation
- Trained the following classification models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Gradient Boosting
  - XGBoost
  - Support Vector Machine
  - K-Nearest Neighbors
- Used a loop to evaluate all models and compare accuracy
- Best model saved using `pickle` 🥒

### 4. 🗃️ Model Saving
- Saved the trained best model (`model.pkl`)
- Saved the preprocessing scaler (`scaling.pkl`)

---

## 🏆 Best Model

✅ **Random Forest Classifier** was selected as the best model based on accuracy and generalization.

---

## 🚀 Deployment (Optional)

This project can be easily deployed using:
- Streamlit for web app UI
- Flask or FastAPI for backend API

---

## 🖼️ Project Cover Image

![Bird Migration Pattern Prediction](A_digital_image_features_migrating_birds_in_mid-fl.png)

---

## 📚 Requirements

Install all dependencies using:

```bash
pip install -r requirements.txt
