TITLE:
Sleep Efficiency Prediction using Machine Learning

OVERVIEW:
This project focuses on predicting sleep efficiency using machine learning techniques based on demographic, behavioral, and sleep-related features. The goal is to analyze how different lifestyle and sleep patterns influence sleep quality.

OBJECTIVES:
- Predict sleep efficiency using ML models  
- Compare performance of multiple regression algorithms  
- Identify key factors affecting sleep quality  
- Analyze model limitations and data challenges

DATASET:
- Contains 1000 records and 15 features  
- After preprocessing: 744 records  
- Features include:
  - Age, Gender  
  - Sleep Duration  
  - REM, Deep, Light Sleep %  
  - Awakenings  
  - Caffeine & Alcohol Consumption  

Target Variable: Sleep Efficiency (continuous value)

DATA PREPROCESSING:
- Removed missing values (CaffeineConsumption column)  
- Encoded categorical variables (Gender, Smoking Status)  
- Applied StandardScaler for feature scaling  
- Performed train-test split (80:20 ratio)

MODELS IMPLEMENTED:
- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Support Vector Regression (SVR)  

EVALUATION METRICS:
- Mean Absolute Error (MAE)  
- Mean Squared Error (MSE)  
- R² Score

RESULTS AND ANALYSIS:
- Linear Regression performed best (lowest MAE & MSE)  
- All models showed negative R² scores, indicating poor predictive performance  
- Decision Tree showed overfitting  
- Random Forest slightly improved results but still weak  
- SVR showed moderate performance but needed tuning  

KEY INSIGHT:
- The dataset lacks strong predictive relationships, affecting model performance  

LIMITATIONS:
- Weak correlation between features and target  
- Important features (stress, screen time, physical activity) missing  
- Reduced dataset size due to missing value removal  
- Limited feature engineering  

CONCLUSION:
- Although multiple models were tested, none achieved strong predictive accuracy  
- This highlights the importance of:
  - Data quality  
  - Feature relevance  
  - Proper model tuning  

FUTURE IMPROVEMENTS:
- Add features like stress levels, physical activity, and screen time  
- Apply feature engineering techniques  
- Perform hyperparameter tuning  
- Use advanced models:
  - Gradient Boosting  
  - XGBoost  
  - Neural Networks  
- Use data imputation instead of dropping rows  

TECH STACK USED:
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib / Seaborn  

