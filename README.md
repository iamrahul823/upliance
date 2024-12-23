
## Analysis Report
### Key Findings:
1. The most popular dish is {popular_dishes.iloc[0]['Dish_Name']} with {popular_dishes.iloc[0]['Count']} orders.
2. There is a positive correlation between the number of cooking sessions and total orders.
3. Users aged {age_location_meal_relation['Age'].iloc[0]} from {age_location_meal_relation['Location'].iloc[0]} prefer {age_location_meal_relation['Favorite_Meal'].iloc[0]} and placed the highest number of orders.
4. Orders are highest during {time_order_relation['Time_of_Day'].iloc[time_order_relation['total_orders'].idxmax()]}. 
5. Higher session ratings are associated with increased orders.

### Recommendations:
- Focus on promoting the top dishes to increase user engagement.
- Target marketing efforts towards locations and age groups with higher order activity.
- Encourage users to cook more by providing incentives, as sessions correlate with orders.
- Optimize platform usage during peak times (e.g., {time_order_relation['Time_of_Day'].iloc[time_order_relation['total_orders'].idxmax()]}).
- Improve session experiences to achieve higher ratings and more orders.

### Visualizations:
- Top 10 Popular Dishes
- Cooking Sessions vs Orders
- Demographic Analysis: Favorite Meals by Location and Age
- Time of Day vs Total Orders
- Session Ratings vs Total Orders
"""




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
