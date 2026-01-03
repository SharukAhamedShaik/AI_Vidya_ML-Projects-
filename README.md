# House Price Prediction with Linear Regression
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
## How to Run
1. Clone this repository:
   bash
   git clone https://github.com/your-username/house-price-linear-regression.git

