# Stock-Price-Prediction

# Project Overview
This project aims to predict stock prices using multiple machine learning models, including:
- K-Nearest Neighbors (KNN)
- XGBoost (XGB)
- Random Forest (RF)
- Linear Regression (LR)

The dataset is preprocessed, analyzed for correlations, and split into training and test sets before model training and evaluation.

 # Dataset
- The dataset is loaded from `stock_data.csv`.
- It includes stock price information for multiple companies over time.
- Features are normalized using MinMaxScaler.

# Data Preprocessing
- The `date` column is converted to datetime format.
- Features are selected based on correlation with `Stock_2`.
- MinMaxScaler is applied for normalization.
- Data is split into **80% training** and **20% testing**.

## Models & Hyperparameter Tuning

### 1️:  K-Nearest Neighbors (KNN)
- Hyperparameters tuned using GridSearchCV:
  - `n_neighbors: [3, 5, 7, 9]`
  - `weights: ['uniform', 'distance']`

### 2️:  XGBoost (XGB)
- Parameters:
  - `n_estimators: [100, 200, 300]`
  - `learning_rate: [0.01, 0.1, 0.2]`
  - `max_depth: [3, 6, 9]`

### 3️: Random Forest (RF)
- Parameters:
  - `n_estimators: [100, 200, 300]`
  - `max_depth: [None, 10, 20, 30]`

### 4️: Linear Regression (LR)
- Simple linear regression model with `fit_intercept` tuning.
- 
## Model Evaluation Metrics
Each model is evaluated using:
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **Mean Absolute Error (MAE)**
- **R-squared Score (R²)**

## Results & Conclusion
- The model with the best performance is selected based on RMSE and R² scores.
- Further improvements can be made with additional feature engineering and hyperparameter tuning.

# Novelty:
Data-Driven Feature Selection: Correlation analysis and feature selection based on it adds a layer of insight to the stock prediction task.

Exploratory Data Analysis: Your pairplot and visualization techniques add depth to understanding the data.

Modeling Diversity: Implementing multiple models (KNN, XGBoost, Random Forest, and Linear Regression) and comparing their performance provides robustness and depth to the project.

Hyperparameter Tuning: Grid search optimization to enhance model performance is a key novelty.

Practical Application: The project tackles a real-world business problem of stock price prediction, making it highly relevant to the financial sector.


##  👩‍💻 Author
Gudepu Rakshitha Reddy

📧 Email: rakshithareddy1985@gmail.com

