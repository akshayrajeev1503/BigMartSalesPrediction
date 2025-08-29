# BigMartSalesPrediction

## Thought process
- Started with data exploration
- Looked at each column
- Fixed irregularities and nulls found in 2 columns
   - Explored different methods to fill missing values
- Started with a simple XGBRFRegressor model to see where I stand and work from there on - 3900 rank! a lot to work on
- Started doing feature engineering - basic interaction features between features I thought are making sense or are intuitive
- Trained LGBM and XGBoost model with new features - these eimproved the rank and rmse but not much
- Enter Catboost - with same features as well - 2900 rank!
- Tuned catboost with optuna - rank under 1200
- Next created advanced features - bins, ratios, counts etc. - tried lots of features: what you see is a cleaned up version
- at this point there are lots of features - so features selection: dont want to give the model less significant features as it will just increase the training time
- trained the catboost model with the new features - Boom! 514 rank
- <img width="1155" height="695" alt="image" src="https://github.com/user-attachments/assets/80ceea25-ef61-4f77-84ad-f9df4e3b5180" />
