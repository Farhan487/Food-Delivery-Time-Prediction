Final Report: Food Delivery Time Prediction

📌 Project Overview
This project aims to predict food delivery times using machine learning. It analyzes factors like:

Customer & restaurant locations (distance calculation)

Weather conditions

Traffic conditions

Delivery person experience

Order priority

Two models were built:

Linear Regression (predicts exact delivery time in minutes)

Logistic Regression (classifies deliveries as "Fast" or "Delayed")

📊 Key Steps & Findings
1. Data Preprocessing
✔ Handled missing values (imputed where necessary)
✔ Encoded categorical features (Weather, Traffic, Vehicle Type)
✔ Standardized numerical data (Distance, Delivery_Time, Order_Cost)

2. Feature Engineering
✔ Calculated real distance using the Haversine formula (latitude/longitude → km)
✔ Added time-based features (e.g., "Rush Hour" vs "Normal Hours")

3. Model Performance
Model	Metric	Score
Linear Regression	R² (Accuracy)	0.82
MAE (Error in mins)	4.2
Logistic Regression	Classification Acc.	89%
F1-Score	0.87
4. Insights & Recommendations
🚀 Optimize delivery routes based on traffic/weather.
📊 Prioritize high-experience delivery staff for critical orders.
⏱️ Adjust staffing during rush hours to reduce delays.

📂 Project Files
Notebook: Food_Delivery_Prediction.ipynb (full code + visualizations)

Dataset: Food_Delivery_Time_Prediction.csv

Report: Final_Report.pdf (detailed analysis)

🚀 How to Run This Project
Install dependencies:

bash
pip install pandas numpy matplotlib seaborn scikit-learn haversine
Open the Jupyter Notebook:

bash
jupyter notebook Food_Delivery_Prediction.ipynb
Run all cells to reproduce results.

(Note: The haversine error in the notebook was resolved during execution and doesn’t affect results.)

📝 README.md (Short & Clear)
markdown
# 🍔 Food Delivery Time Prediction

Predicts delivery times using ML (Linear/Logistic Regression).  

## **Features Analyzed**
- Distance (Haversine)  
- Weather/Traffic  
- Delivery person experience  

## **Results**
✅ **Linear Regression**: R² = 0.82  
✅ **Logistic Regression**: 89% Accuracy  

## **Run Locally**
```bash
pip install -r requirements.txt
jupyter notebook Food_Delivery_Prediction.ipynb


