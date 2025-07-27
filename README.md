# Churn-Rate-Predictor-Ensemble-Methods
This is a Churn rate Classifier using Ensemble Methods. Check out the output of the code.... The time taken has also been showed to show the tradeoff between F1 Score with Computational Complexity

# Customer Churn Prediction Using Ensemble Learning

This project focuses on applying various ensemble learning techniques to predict customer churn. Multiple models are trained, evaluated, and compared based on metrics such as accuracy, F1 score, and training time.

## Dataset

- **Source**: Bank Customer Churn Dataset (Kaggle)
- **Target Variable**: `churn` (binary classification)
- **Features**: Includes customer demographics, account activity, and services used.

## Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- AdaBoost
- Bagging (with Random Forest)
- Gradient Boosting
- Histogram-Based Gradient Boosting
- XGBoost
- Voting Classifier (Soft Voting with top models)

## Preprocessing

- Handled categorical and numerical features appropriately
- Applied `StandardScaler` for models sensitive to feature scaling (like Logistic Regression)
- Used `train_test_split` with stratification on the target variable

## Evaluation Metrics

- Accuracy Score
- F1 Score
- Confusion Matrix
- Training Time

All models were evaluated on the same test set and their results compiled into a pandas DataFrame for comparison.

## Results

Models were compared based on:
- Accuracy
- F1 Score (used for final sorting)
- Time taken to train and predict

The final results table was sorted by F1 Score to identify the best-performing models in terms of both performance and reliability.

## Visualization

- Confusion matrices were plotted for each model
- Clear visual insights into false positives/negatives and overall performance

## Key Observations

- Ensemble methods generally outperformed individual classifiers
- Histogram-Based and Gradient Boosting models gave strong results with relatively fast training times
- Voting Classifier combining Random Forest, HGBT, and Logistic Regression performed competitively
- Logistic Regression required scaling and more iterations to converge properly
