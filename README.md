# 🌧️ Stormwater Optimization with Blue Roofs

This project analyzes rainfall, storm sewer, and pipe data to simulate stormwater retention **with and without blue roof systems**. Using **machine learning** and **spatial analysis**, it predicts water release decisions, quantifies stormwater savings, and visualizes rainfall patterns to support sustainable urban drainage planning.

---

## 🚀 Overview
Urban flooding is a growing challenge in cities like Toronto due to **climate change** and **rapid urbanization**. This project provides a **data-driven solution** that evaluates how much stormwater can be retained using blue roofs — which store water temporarily to prevent sewer system overloads.

Our workflow integrates and models open environmental data to optimize stormwater management and improve resilience in urban infrastructure.

---

## 🧠 Key Features
- 🌧️ Integrates rainfall, storm sewer, and pipe datasets  
- 📍 Performs **spatial matching** of rainfall to sewer nodes using `SciPy KDTree`  
- ⚙️ Engineers features like **Node Capacity** based on rainfall intensity and temperature  
- 🤖 Trains a **Random Forest Classifier** to predict release decisions  
- 💧 Quantifies **stormwater retained** by blue roofs under different rainfall scenarios  
- 📊 Visualizes rainfall trends and system responses with `Matplotlib`  
- 🧾 Exports processed and predicted data as CSV and JSON for reporting  

---

## 🧰 Tech Stack
- **Language:** Python 3.x  
- **Libraries:** pandas, NumPy, SciPy, scikit-learn, Matplotlib, JSON  
- **Data Source:** Toronto Open Data — Rainfall, Storm Sewer Nodes, Storm Sewer Pipes  

---

## 📂 Repository Structure
<img width="757" height="170" alt="image" src="https://github.com/user-attachments/assets/0af1dd09-effc-4f58-a1e1-5f8bc74b18ed" />

---

## 📊 Workflow Summary
1. **Data Preprocessing**  
   Standardized column names, cleaned missing values, extracted month and temperature data.  
2. **Spatial Matching**  
   Matched rainfall events to nearest storm sewer nodes using `SciPy.cKDTree`.  
3. **Feature Engineering & Modeling**  
   Created `Node_Capacity` feature and trained a `RandomForestClassifier` with cross-validation.  
4. **Prediction & Evaluation**  
   Predicted stormwater release decisions and calculated model accuracy.  
5. **Visualization & Reporting**  
   Generated rainfall vs. release plots and calculated total stormwater retained.  

