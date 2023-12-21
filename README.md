# Calories Burnt Prediction

This Python code uses the XGBoost (Extreme Gradient Boosting) regression model to predict calorie expenditure based on various features from an exercise dataset. Here's a breakdown of the code:

1. **Import Libraries:**
   - `numpy` and `pandas` for data manipulation
   - `matplotlib.pyplot` and `seaborn` for data visualization
   - `train_test_split` from `sklearn.model_selection` to split the dataset into training and testing sets
   - `XGBRegressor` from `xgboost` for building and training the XGBoost regression model
   - `metrics` from `sklearn` to evaluate the model performance

2. **Read Data:**
   - Reads an exercise dataset from a CSV file using Pandas.
   - Displays the first few rows, general information, and summary statistics of the dataset.

3. **Data Cleaning and Preparation:**
   - Checks for null values in the dataset.
   - Converts the 'Gender' column values ('male' and 'female') to numerical values (0 and 1).
   - Concatenates the 'Calories' column from a separate 'calories.csv' file to the exercise dataset.
   - Drops the 'User_ID' column from the dataset.

4. **Data Exploration:**
   - Computes the correlation matrix of the dataset and visualizes it using a heatmap.

5. **Data Visualization:**
   - Displays distribution plots for the 'Age', 'Height', 'Weight', 'Duration', and 'Heart_Rate' columns.

6. **Feature and Target Split:**
   - Divides the dataset into features (X) and the target variable (Y).

7. **Train-Test Split:**
   - Splits the data into training and testing sets (80% training, 20% testing).

8. **XGBoost Model Training:**
   - Initializes an XGBoost regressor.
   - Fits the regressor to the training data.

9. **Model Evaluation on Training Set:**
   - Predicts calorie expenditure on the training set.
   - Computes the R-squared score for the training set.

10. **Model Evaluation on Testing Set:**
   - Predicts calorie expenditure on the testing set.
   - Computes the R-squared score for the testing set.

11. **Display Results:**
   - Displays a subset of predicted values and actual values from the testing set.

Overall, this code explores and prepares an exercise dataset, builds an XGBoost regression model, and evaluates its performance on predicting calorie expenditure. The evaluation includes examining the R-squared score on both the training and testing sets.
