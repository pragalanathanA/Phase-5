# README for IMDb Score Prediction

This code is an example of predicting IMDb scores using a linear regression model.

1. Data Loading and Exploration: The code loads a CSV dataset named "result.csv" using Pandas and displays the first few rows with `print(p.head())`.

2. Data Cleaning: Missing values and duplicate rows are removed from the dataset with `p.dropna(inplace=True)` and `p.drop_duplicates(inplace=True)`.

3. Data Transformation: The 'UnEmployeeRate' and 'movieScore' columns are converted to numeric data types, ensuring they are suitable for modeling.

4. Data Filtering: The dataset is filtered to select relevant features ('year', 'UnEmployeeRate', and 'movieScore') for the prediction task.

5. Train-Test Split: The dataset is split into training and testing sets using `train_test_split` from Scikit-Learn. 80% of the data is used for training the linear regression model.

6. Model Training: A linear regression model is created and trained on the training data with `model.fit(X_train, y_train)`.

7. Model Evaluation: The model's performance is evaluated by predicting 'year' on the test set and calculating the Mean Squared Error (MSE) with `mean_squared_error`. The MSE is printed to assess the model's predictive accuracy.

