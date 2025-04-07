# 🌆 Delhi AQI Prediction using Machine Learning

This project aims to predict the **Air Quality Index (AQI)** of **Delhi, India** using various machine learning models. With the rise in pollution, especially in metro cities, this project demonstrates how data science can be leveraged to forecast AQI and assist in timely interventions.

---

## 📌 Project Overview

- **Goal**: Predict daily AQI in Delhi using historical pollution data.
- **Approach**: Data cleaning, feature engineering, model training, evaluation, and model saving.
- **Dataset**: [Air Quality Data in India (2015-2020)](https://www.kaggle.com/datasets/vopani/air-quality-data-in-india) by Vopani (filtered for Delhi).

---

## 📁 Folder Structure

delhi-aqi-prediction/ │ ├── data/ │ ├── raw/ # Contains original city_day.csv │ └── processed/ # Contains cleaned delhi_daily_aqi.csv │ ├── models/ │ └── xgboost_aqi_model.pkl # Saved trained model │ ├── plots/ # Visualizations used in notebook & README │ ├── AQI_distribution.png │ └── Performace_matrix_comparison.png │ ├── requirements/ │ └── requirements.txt # Python dependencies │ ├── Delhi_AQI_Prediction.ipynb # Main notebook └── README.md

yaml
Copy
Edit

---

## 🧠 Concepts & Technologies Used

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Supervised Learning (Regression)
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
- Evaluation Metrics: MAE, RMSE, R²
- Model Saving with `joblib`
- Project Structuring
- Visualizations with Matplotlib & Seaborn

---

## 📊 Sample Visualizations

### AQI Distribution Across Time:
![AQI Distribution](plots/AQI_distribution.png)

### Model Performance Comparison:
![Performance Matrix](plots/Performace_matrix_comparison.png)

---

## ✅ Best Performing Model

After evaluating multiple models, **XGBoost Regressor** emerged as the best with:

- **Lowest MAE & RMSE**
- **Highest R² Score**
- Robust to overfitting and missing values

---

## 📝 Steps Followed

1. Load and filter the Delhi data from city_day.csv
2. Handle missing values using mean/mode imputation
3. Extract useful features like month, day, etc.
4. Train multiple regression models
5. Evaluate performance using MAE, RMSE, and R²
6. Select the best model (XGBoost)
7. Save the model using joblib
8. Store visualizations in `/plots/` folder

---

## ⚙️ How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/delhi-aqi-prediction.git
Install dependencies:

bash
Copy
Edit
pip install -r requirements/requirements.txt
Open Delhi_AQI_Prediction.ipynb in Jupyter Notebook or Google Colab

Run the cells step-by-step

🧑‍💻 About Me
Akash Sharma
📧 Email: akashsharmatnp@gmail.com
🔗 LinkedIn: linkedin.com/in/akashsharma16

🚀 Future Scope
Integrate real-time AQI data using API

Add weather data for better predictions

Deploy model as a web app using Streamlit or Flask

Send notifications when AQI goes beyond threshold

📌 Final Notes
This project is designed to showcase a full data science workflow using a real-world environmental problem. It includes everything from data acquisition to model saving and performance visualization—ideal for portfolios and interviews!

⭐ If you found this project helpful, consider giving it a star on GitHub and connect with me on LinkedIn!