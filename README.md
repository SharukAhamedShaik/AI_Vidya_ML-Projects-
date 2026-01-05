1) House Price Prediction with Linear Regression
## Dataset
- Source: https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction
- Rows: 545
- Columns: 13
  - price (target)
  - area, bedrooms, bathrooms, stories, parking
  - mainroad, guestroom, basement, hotwaterheating, airconditioning, prefarea, furnishingstatus
## Steps Followed
1. Loaded the dataset and inspected structure using "head()", "info()" and "describe()".
2. Checked and handled missing values.
3. Defined `price` as the target variable and the remaining columns as features.
4. One-hot encoded categorical variables:
   - mainroad, guestroom, basement, hotwaterheating,
     airconditioning, prefarea, furnishingstatus.
5. Split the data into training and testing sets using "train_test_split".
6. Built a Linear Regression model with scikit-learn and trained it on the training data.
7. Generated predictions on the test data.
8. Evaluated the model using R² score and Mean Absolute Error(MAE).
9. Interpreted the results and discussed model performance.
#2) Advanced Model: XGBoost Regression
- Added an **XGBoost Regressor** using the same features and train–test split as Linear Regression.
- Used parameters like `n_estimators=200`, `learning_rate=0.3`, `max_depth=3`, `subsample=0.8`, `colsample_bytree=0.8`.
## Model Performance Comparison
- Difference in R² (XGBoost − Linear): **-0.06** → XGBoost has **lower R²**.
- Difference in MAE (Linear − XGBoost): **-90,284.221** → XGBoost has **higher error**.
- **Linear Regression performed better** overall on this dataset.
## Key Insights
- The **simpler Linear Regression** model worked better than the more complex XGBoost model.
- On this small, structured dataset, XGBoost likely **overfit** and did not generalize as well.
- Linear Regression is **faster, easier to interpret**, and in this case also **more accurate**, so it is the preferred model for this project.
