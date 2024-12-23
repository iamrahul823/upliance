# Predictive Analysis Report

## Objective
The goal of this analysis was to predict the number of total orders placed by users based on their activity and demographic features, using various regression models.

## Key Models and Results

### 1. Linear Regression
- **Mean Absolute Error**: {mean_absolute_error(y_test, y_pred_linear):.4f}
- **Mean Squared Error**: {mean_squared_error(y_test, y_pred_linear):.4f}
- **R² Score**: {r2_score(y_test, y_pred_linear):.4f}

### 2. Ridge Regression
- **Mean Absolute Error**: {mean_absolute_error(y_test, y_pred_ridge):.4f}
- **Mean Squared Error**: {mean_squared_error(y_test, y_pred_ridge):.4f}
- **R² Score**: {r2_score(y_test, y_pred_ridge):.4f}

### 3. Lasso Regression
- **Mean Absolute Error**: {mean_absolute_error(y_test, y_pred_lasso):.4f}
- **Mean Squared Error**: {mean_squared_error(y_test, y_pred_lasso):.4f}
- **R² Score**: {r2_score(y_test, y_pred_lasso):.4f}

### 4. Random Forest Regression
- **Mean Absolute Error**: {mean_absolute_error(y_test, y_pred_rf):.4f}
- **Mean Squared Error**: {mean_squared_error(y_test, y_pred_rf):.4f}
- **R² Score**: {r2_score(y_test, y_pred_rf):.4f}

## Feature Importance (Random Forest)
The most influential features in predicting total orders are:
1. **{feature_importances.iloc[0]['Feature']}**: Importance {feature_importances.iloc[0]['Importance']:.4f}
2. **{feature_importances.iloc[1]['Feature']}**: Importance {feature_importances.iloc[1]['Importance']:.4f}
3. **{feature_importances.iloc[2]['Feature']}**: Importance {feature_importances.iloc[2]['Importance']:.4f}

## Recommendations
1. Focus on increasing user engagement by boosting cooking sessions, as it is the most predictive factor for orders.
2. Optimize platform features to cater to users with higher average session ratings.
3. Use Random Forest predictions for further marketing insights, given its high performance and feature interpretability.

## Visualizations
- Actual vs Predicted Orders (Random Forest)
- Feature Importance (Random Forest)
""")
