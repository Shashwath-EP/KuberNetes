NYC Taxi Fare Prediction


This project builds a Machine Learning model to predict taxi fare amounts in New York City based on various features like distance, time, and location coordinates.The goal is to develop a model that accurately predicts taxi fares, assisting taxi companies or services in setting competitive and fair pricing.

Table of Contents

Project Description
Dataset
Project Setup
Model Training and Evaluation
Usage
Evaluation Metrics
Visualization
Technologies

Project Description

This project leverages supervised machine learning techniques to predict NYC taxi fares. It utilizes the NYC Taxi Fare Prediction dataset from Kaggle and preprocesses data to include features like pickup and drop-off coordinates, time of day, distance, and more.

Dataset

The dataset used is from the Kaggle competition New York City Taxi Fare Prediction. It includes details such as pickup and drop-off coordinates, timestamp, and the fare amount for each trip.

Features:

pickup_datetime: Timestamp of the pickup time
pickup_longitude, pickup_latitude: Pickup coordinates
dropoff_longitude, dropoff_latitude: Drop-off coordinates
passenger_count: Number of passengers in the trip


Project Setup

Install required Python packages:

pip install -r requirements.txt


Download the Kaggle dataset:

Place kaggle.json (Kaggle API token) in ~/.kaggle/.



Model Training and Evaluation:

Data Preprocessing: Clean and filter the dataset, removing unrealistic values and outliers.

Feature Engineering: Calculate distance_km between pickup and drop-off points.Extract time-related features like hour, day, and day of the week.

Model Training: Train a Random Forest Regressor on the processed data.

Evaluation: Calculate evaluation metrics such as RMSE, MAE, R2 Score,  and visualize the model’s performance.


Evaluation Metrics

The model is evaluated based on:

RMSE (Root Mean Squared Error): Measures the average error magnitude in dollars.

MAE (Mean Absolute Error): Indicates the average absolute error magnitude.

R² Score: Represents the goodness of fit of the model.


Additional Metrics and Visualizations:

MAPE (Mean Absolute Percentage Error): Provides percentage error insights.

Residuals Plot: Shows the residual distribution.

Actual vs. Predicted Plot: Visualizes actual vs. predicted fare amounts.

Feature Importance Plot: Highlights key features influencing the prediction.


Visualization

Generated visualizations include:

Residuals Distribution: To check for bias in the model.

Scatter Plot of Actual vs. Predicted: To analyze model prediction quality.

Feature Importance Plot: (specific to Random Forest) to identify the most influential features.


Technologies


Python: Programming language
Pandas: Data manipulation and analysis
Scikit-Learn: Machine learning visualization library
Geopy: For calculating geographical distances
Matplotlib & Seaborn: For data visualization

