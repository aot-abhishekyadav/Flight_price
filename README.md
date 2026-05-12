# Flight_price
# Flight Price Prediction Project ✈️
# Project Overview
This project is based on Machine Learning for Flight Fare Prediction using Python.
The main objective of this project is to predict airline ticket prices based on different factors such as airline, journey date, source, destination, stops, duration, departure time, and arrival time.
The dataset was cleaned, transformed, and processed using Feature Engineering techniques, and different Machine Learning algorithms were applied to achieve accurate predictions.

# Technologies Used
. Python
. NumPy
. Pandas
. Matplotlib
. Seaborn
. Scikit-learn
. Google Colab

# Dataset Information
The project uses two datasets:
1. Training Dataset
. Contains flight details along with ticket prices.
. Used to train the model.

2.Testing Dataset
. Contains flight details without prices.
. Used for prediction/testing.

# Features in Dataset
. Airline
. Date_of_Journey
. Source
. Destination
. Route
. Dep_Time
. Arrival_Time
. Duration
. Total_Stops
. Additional_Info
. Price (Target Variable)

# Data Preprocessing & Feature Engineering
Several preprocessing steps were performed to clean and prepare the dataset:
1. Date Processing
. Extracted:
   . Journey Date
   . Journey Month
   . Journey Year

2. Arrival Time Processing
. Extracted:
   . Arrival Hour
   . Arrival Minute

3. Departure Time Processing
. Extracted:
   . Departure Hour
   . Departure Minute

4. Duration Processing
. Converted flight duration into:
    . Duration Hours
    . Duration Minutes
    . Total Duration in Minutes

5. Handling Missing Values
. Filled missing values in:
    . Total_Stops
    . Duration_Minutes
    . Removed invalid rows

6. Categorical Encoding
. Used Label Encoding to convert categorical columns into numerical format:
   . Airline
   . Source
   . Destination
   . Additional_Info

# Machine Learning Models Used

1. Linear Regression
 . Linear Regression was used as the baseline model.
-> Result
. R² Score: 0.307
This model gave lower accuracy because flight price prediction is a nonlinear problem.

2. Random Forest Regressor
 . Random Forest Regressor was used to improve prediction performance.
-> Result
. R² Score: 0.865
Random Forest performed significantly better and achieved high prediction accuracy.

# Model Performance Comparison
Model                          R² Score
Linear Regression              0.307
Random Forest Regressor        0.865

# Project Workflow
1. Import Libraries
2. Load Dataset
3. Data Cleaning
4. Feature Engineering
5. Handle Missing Values
6. Encode Categorical Features
7. Train-Test Split
8. Train Models
9. Evaluate Models
10. Compare Results

# Key Learnings
. Data preprocessing is very important in Machine Learning.
. Feature engineering improves model performance.
. Random Forest works well for nonlinear regression problems.
. Proper handling of missing values increases prediction accuracy.

# Conclusion
This project successfully predicts flight ticket prices using Machine Learning techniques.
Among all models used, Random Forest Regressor provided the best performance with an R² score of 0.865, making it highly effective for fare prediction tasks.
