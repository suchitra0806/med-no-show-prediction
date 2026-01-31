# 🏥 HealthPredict: Medical Appointment No-Show Analysis

This project uses machine learning to predict the likelihood of a patient missing their medical appointment. By identifying potential "no-shows," healthcare providers can optimize scheduling and improve patient care delivery.

## 🚀 Project Overview
Medical no-shows cost the healthcare system billions and delay care for patients in need. I built a **random forest classifier** to analyze 110k+ records and predict attendance based on patient demographics and appointment history.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** Pandas, Scikit-learn, Matplotlib, Seaborn

## 📈 Key Findings & Model Optimization
- **Feature Importance:** The most significant predictor was `WaitTime` (the number of days between booking and the actual appointment).
- **Handling Imbalance:** The original dataset had far more "shows" than "no-shows." I implemented `class_weight='balanced'` to ensure the model didn't ignore the minority class.
- **Results:** By tuning the model,  increased the **recall for no-shows by 63%**, significantly improving the model's clinical utility.