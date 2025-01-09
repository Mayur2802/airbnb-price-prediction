# Airbnb Price Prediction

This repository contains a machine learning project aimed at predicting house prices based on a variety of features. The project was originally developed as part of a Kaggle competition, where the test dataset was hidden for evaluation purposes. The repository demonstrates preprocessing, feature engineering, model development, and evaluation.

## Features
- Preprocessing of data (handling missing values, outliers, and scaling)
- Feature engineering (label encoding, tokenization, and vectorization using TF-IDF and Word2Vec)
- Training and evaluating models:
  - Lasso Regression
  - Regression Tree
  - XGBoost Regressor
- Hyperparameter tuning using Grid Search
- Scoring models on validation data
- Generating predictions for a test dataset (no `y_test` available)

## Repository Structure
- `notebooks/`: Contains the Jupyter notebook used for the workflow.
- `data/`: Dataset files.
- `README.md`: Project documentation.
- `requirements.txt`: Necessary libraries for the project

## Data Description
The dataset contains:
- **Features:** Information about houses (e.g., size, location, number of rooms).
- **Target:** The sale price of houses (for training data only).
- **Note:** The test dataset used for final evaluation is hidden.

## Installation and Requirements
1. Clone the repository: 
2. Requirements: pip install -r requirements.txt

## Project Workflow
1. **Preprocessing:**
   - Handled missing values, outliers, and scaling.
2. **Feature Engineering:**
   - Applied label encoding, tokenization, and vectorization (TF-IDF and Word2Vec) to process categorical and text-based features.
3. **Model Training:**
   - Trained and evaluated multiple models:
     - Lasso Regression
     - Regression Tree
     - XGBoost
   - Used Grid Search for hyperparameter optimization.
4. **Evaluation:**
   - Calculated RMSE and \( R^2 \) scores on the validation set for each model.
5. **Test Predictions:**
   - Generated predictions for the test dataset for submission to Kaggle.
   - Note: Test metrics cannot be calculated as `y_test` is unavailable.

## Results
XGBoost achieved the best performance among the models. The performance of all three models can be further improved by finessing the data preprocessing and feature engineering parts. 

## Limitations
- Metrics for the test set cannot be calculated as `y_test` was hidden for competition evaluation.
- Additional feature engineering or ensemble models could potentially improve results.

## How to Use This Repository
1. Clone the repository and set up the required environment as mentioned in the Installation section.
2. Navigate to the `notebooks/` directory to explore the Jupyter notebook.
3. Modify and experiment with the code to test alternative workflows or models.

