# Dubai-Weather-Rain-Prediction-ML-
Machine learning project that predicts whether it will rain tomorrow in Dubai using historical weather data, time-series feature engineering, and a Random Forest classifier.

Dubai Weather Rain Prediction using Machine
Learning
Project Objective
This project builds a Machine Learning model to predict whether it will rain tomorrow in Dubai using
historical daily weather data. The task is treated as a binary classification problem (Rain / No Rain).
Dataset Overview
The dataset contains long-term daily Dubai weather records including date, minimum temperature,
maximum temperature, average temperature, and precipitation.
Rain labels are derived from precipitation values where precipitation greater than zero is treated as
rain.
Data Preprocessing Steps
• Converted date column to datetime format
• Sorted records chronologically
• Normalized column names
• Dropped irrelevant columns
• Handled missing values using interpolation and forward/backward fill
• Removed rows created as NaN after lag feature creation
Feature Engineering
Time-series and derived features were created to improve prediction quality.
• Temperature range (max minus min)
• Average temperature lag features (1-day and 3-day)
• Previous rain indicator
• Rolling rain count over last 3 days
• Month and day-of-year seasonal features
Machine Learning Model
A Random Forest Classifier is used for prediction because it performs well on tabular data, handles
nonlinear relationships, and is robust to noise.
Balanced class weights are used to handle rare rain events.
Class Imbalance Handling
Rain days are rare in Dubai, so the dataset is highly imbalanced. The model uses balanced class
weights and evaluation metrics beyond accuracy such as precision, recall, and F1-score.
Evaluation Metrics
• Precision
• Recall
• F1 Score
• Confusion Matrix
How to Run
• Open Google Colab
• Upload the dataset CSV file
• Run cleaning, feature engineering, training, and evaluation cells in order
Tech Stack
• Python
• Pandas
• Scikit-learn
• Matplotlib
• Google Colab
• Random Forest Algorithm
Learning Outcomes
• Time-series preprocessing
• Missing value handling
• Lag and rolling feature engineering
• Binary classification modeling
• Handling imbalanced datasets
• ML evaluation beyond accuracy

AUTHOR 
Amaan Haroon — Machine Learning & AI Enthusiast
