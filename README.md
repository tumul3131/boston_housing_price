# Housing Price Prediction

This project involves predicting housing prices using a publicly available dataset such as the Boston Housing dataset or the California Housing dataset. The workflow includes data collection, preprocessing, model development, and model evaluation.

## Requirements

### 1. Data Collection
- Use a publicly available dataset such as the Boston Housing dataset or the California Housing dataset.
- The column names for the dataset are as follows:
  ```python
  column_names = ['CRIM', 'ZN', 'INDUS', 'CHAS', 'NOX', 'RM', 'AGE', 'DIS', 'RAD', 'TAX', 'PTRATIO', 'B', 'LSTAT', 'MEDV']
  ```

### 2. Data PreProcessing
- The column name was given to get the features.
  ```python
  df=pd.read_csv('housing.csv',header=None,sep='\s+',names=column_names)
  ```
- No missing values found in the dataset.
- Feature Scaling was performed using Standardisation.
- The train and test data spliting was done to train the data separately on models.

### 3. Model Development
- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- XGBoost Regression

### 4. Model Evaluation
- R2 Score :
  - R² = 1: The model perfectly predicts the data.
  - R² = 0: The model does no better than the mean of the dependent variable.
  - R² < 0: The model is worse than a horizontal line through the mean of the dependent variable.
   # A very high R² (close to 1) suggests a good fit.
- Mean Absolute Error:
  A lower MAE value indicates a better fit.
- Mean Squared Error:
  A lower MSE indicates a better fit.

