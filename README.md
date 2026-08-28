# Prediction of Agriculture Crop Production in India

## About the Project

This project focuses on predicting agriculture crop production in India using Machine Learning.

Historical crop production data was processed and used to train machine learning regression models. Previous-year production, area, and yield information were used to predict the production of the following year.

## Objective

The main objective of this project is to develop a machine learning model that can predict crop production using historical agricultural data.

## Dataset

The dataset contains information about different crops for the years 2006-07 to 2010-11.

The main attributes used in the project are:

- Crop
- Year
- Production
- Area
- Yield

The original dataset was converted into a structured format suitable for machine learning.

## Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the agriculture dataset.
2. Cleaned the column names.
3. Converted the original yearly data into an ML-friendly format.
4. Checked for missing values.
5. Created previous-year production, area, and yield features.
6. Removed records where previous-year information was unavailable.
7. Prepared input features and target variable.

## Machine Learning Approach

The model uses previous-year agricultural information to predict the next year's crop production.

### Input Features

- Previous Production
- Previous Area
- Previous Yield

### Target

- Production

The processed dataset contained 220 records for machine learning.

The data was divided into:

- Training data: 176 records
- Testing data: 44 records

## Machine Learning Models

Two regression models were tested:

1. Linear Regression
2. Random Forest Regression

## Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Linear Regression

- MAE: 28.32
- RMSE: 40.86
- R² Score: 0.76

### Random Forest Regression

- MAE: 30.26
- RMSE: 41.10
- R² Score: 0.76

## Final Model

Linear Regression was selected as the final model because it achieved a lower MAE and RMSE than Random Forest while achieving the same R² score.

## Result

The final Linear Regression model achieved an R² score of 0.76 on the test data.

An Actual vs Predicted Crop Production graph was also created to visualize the model predictions.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab
- Jupyter Notebook

## Project Files

- `agriculture_crop_prediction.ipynb` - Machine learning implementation
- `crop_production_model.pkl` - Trained Linear Regression model
- `processed_crop_data.csv` - Processed dataset
- `crop_production_predictions.csv` - Prediction results
- `actual_vs_predicted.png` - Model evaluation graph

## Conclusion

The project demonstrates how historical agricultural data can be processed and used to build a machine learning regression model for crop production prediction.

Linear Regression provided the best performance among the tested models and was selected as the final model.
