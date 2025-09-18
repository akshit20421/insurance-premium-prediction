# 📊 Insurance Premium Prediction using GLM

## 📌 Overview
This project predicts **health insurance premiums** using a **Generalized Linear Model (GLM)** with a Gamma distribution and log link.  
The goal was to replicate an **actuarial pricing framework** and derive business insights from health insurance data.

## 📂 Dataset
- Dataset contains **1M+ health insurance records** with demographic and lifestyle attributes.  
- Features: age, gender, BMI, smoking status, region, charges, etc.  
- Source: Kaggle – Health Insurance Dataset.  

## ⚙️ Methodology
1. **Data Preprocessing**
   - Cleaned dataset, handled missing values.  
   - Feature engineering (age bands, smoker flag, premium coverage indicator).  

2. **Model Development**
   - Applied **GLM (Gamma with log link)** for severity modeling.  
   - Fitted charges against key features (age, BMI, smoker, coverage).  

3. **Premium Calculation**
   - Suggested premiums using **20% loading** on predicted charges.  
   - Performed **sensitivity analysis** at +10%, +20%, +30%.  

4. **Validation**
   - Calibration across deciles (error < ±4%).  
   - Predicted mean (₹16,744) closely matched actual mean (₹16,735).  

## 📈 Key Results
- Predicted mean charges: **₹16,744**  
- Actual mean charges: **₹16,735**  
- Suggested premium (20% loading): **₹20,093**  
- **Insights:**  
  - Smokers → ~36% higher charges  
  - Premium coverage → ~35% higher cost than basic  
  - BMI → +0.3% cost increase per unit  

## 🛠️ Tech Stack
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Statsmodels, Matplotlib  
- **Tools:** Jupyter Notebook, Google Colab  

## 👥 Team Members
- Akshit Gupta  
- Ushali Gangwani  
