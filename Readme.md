# 🏥 healthpredict: medical appointment no-show analysis

this project uses machine learning to predict the likelihood of a patient missing their medical appointment. by identifying potential "no-shows," healthcare providers can optimize scheduling and improve patient care delivery.

## 🚀 project overview
medical no-shows cost the healthcare system billions and delay care for patients in need. i built a **random forest classifier** to analyze 110k+ records and predict attendance based on patient demographics and appointment history.

## 🛠️ tech stack
- **language:** python
- **libraries:** pandas, scikit-learn, matplotlib, seaborn
- **environment:** google colab / vscode

## 📈 key findings & model optimization
- **feature importance:** the most significant predictor was `WaitTime` (the number of days between booking and the actual appointment).
- **handling imbalance:** the original dataset had far more "shows" than "no-shows." i implemented `class_weight='balanced'` to ensure the model didn't ignore the minority class.
- **the results:** by tuning the model, i increased the **recall for no-shows by 63%**, significantly improving the model's clinical utility.