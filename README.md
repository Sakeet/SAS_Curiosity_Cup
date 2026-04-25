# SAS_Curiosity_Cup

# 🏥 Frontline Forecast: Hospital Length of Stay Prediction

## 📌 Project Overview
Hospitals constantly struggle to balance patient demand with limited capacity.  
Even small errors in estimating how long a patient will stay can lead to:
- Overcrowding  
- Wasted resources  
- Delays in care  

This project focuses on predicting **Length of Stay (LOS)** for diabetic patients and, more importantly, translating those predictions into **actionable decisions** for hospital operations.

Our goal is not just prediction — but **better decision-making**.

---

## 📊 Dataset

This project uses the publicly available UCI dataset:

- **Source:** UCI Machine Learning Repository  
- **Dataset:** Diabetes 130-US hospitals (1999–2008)  
- **Link:** https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008  

- **Size:** 101,766 patient encounters  
- **Hospitals:** 130 U.S. hospitals  


> ⚠️ The dataset is not included in this repository due to size and licensing considerations.

---

## 🧠 Approach

Instead of relying on a single model, we used multiple approaches to improve both **prediction accuracy** and **practical usefulness**:

### 1. Regression — Predict Length of Stay
Estimate how many days a patient is likely to stay in the hospital.

### 2. Classification — Identify Long vs Short Stays
Helps prioritize patients who may require more resources.

### 3. Uncertainty Estimation (Quantile Regression)
Instead of predicting a single number, we provide a **range** (e.g., 2–6 days),  
similar to a weather forecast — more useful for planning.

### 4. Simulation — From Prediction to Decision
We simulate real-world hospital scenarios to understand how predictions affect bed allocation and operational efficiency.

---

## 📈 Key Results

- **Best Model:** LightGBM  
- **Mean Absolute Error (MAE):** ~1.60 days  
- **Long-stay classification accuracy:** 78.3%  
- **Uncertainty coverage:** ~80% (well-calibrated prediction ranges)

---

## 🔍 What-If Scenario (Operational Impact)

We tested a simple but powerful scenario:

👉 **If 10% of patients are discharged 1 day earlier:**

- Peak bed demand reduces by **8–12 beds per day**  
- Equivalent to **~4–5% capacity relief**

---

## 💡 Key Insights

- **Clinical complexity drives unpredictability**, not demographics  
- **Number of medications is the strongest predictor** of longer stays  
- Early discharge is **partially predictable**, but not perfect  
- **Small operational changes can create significant system-wide impact**

---

## 👥 Team

**Frontline Forecast**  
University of North Texas  

- Kate Dau  
- Aarya Acharya  
- Sakeet Kopparapu  
- Sulav Regmi  

**Faculty Advisor:**  
- Professor Michel Fathi  

---

## 📎 Additional Resources

📘 Project notebook: [SAS_Combined.ipynb](./SAS_Combined.ipynb)  
📄 Final report: [SAS_Curiosity_Cup_Final_Submission.pdf](./SAS_Curiosity_Cup_Final_Submission.pdf)


Thank you for your interest!
