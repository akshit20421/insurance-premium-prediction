# Insurance Premium Prediction using GLM

## 📌 Overview
This project predicts **health insurance premiums** using a **Generalized Linear Model (GLM)** with a Gamma distribution and log link.  
The goal is to replicate an actuarial-style pricing framework and provide insights into key risk drivers affecting insurance costs.  

## 📊 Dataset
- Health insurance dataset with **1M+ records** (age, gender, BMI, smoking status, region, charges, etc.)  
- Preprocessed and cleaned for modeling.  
- Source: Kaggle (Health Insurance Dataset).  

## ⚙️ Methodology
1. **Data Preprocessing**
   - Handling missing values, feature engineering (age bands, smoker flag, etc.)
   - Outlier and anomaly checks  

2. **Model Development**
   - Applied **GLM (Gamma with log link)** for severity modeling  
   - Fitted medical charges against age, BMI, smoking status, and coverage type  

3. **Premium Calculation**
   - Designed a **premium framework** with 20% loading on predicted charges  
   - Conducted **sensitivity analysis** at +10%, +20%, +30%  

4. **Model Validation**
   - Calibration across deciles (error < ±4%)  
   - Compared predicted vs actual mean charges (16,744 vs 16,735 INR)  

## 📈 Key Results
- Predicted mean charges: **₹16,744**  
- Actual mean charges: **₹16,735**  
- Suggested premium (20% loading): **₹20,093**  
- Key insights:
  - Smokers → ~36% higher charges  
  - Premium coverage → ~35% higher cost than basic  
  - BMI → +0.3% cost increase per unit  

## 🛠️ Tech Stack
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Statsmodels, Matplotlib  
- **Tools:** Jupyter Notebook, Google Colab  

## 📄 Project Structure
