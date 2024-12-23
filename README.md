


#  Analysis Report

## Objective
The goal of this analysis was to predict the number of total orders placed by users based on their activity and demographic features, using various regression models.

## Key Findings:
1. The most popular dish is `Pasta Alfredo` with 152 orders.
2. There is a positive correlation between the number of cooking sessions and total orders.
3. Users aged 32 from `New York` prefer `Chicken Tikka` and placed the highest number of orders.
4. Orders are highest during `Dinner` time.
5. Higher session ratings are associated with increased orders.

## Key Models and Results

### 1. Linear Regression
- **Mean Absolute Error**: 1.2451
- **Mean Squared Error**: 0.5542
- **R² Score**: 0.8943

### 2. Ridge Regression
- **Mean Absolute Error**: 1.2315
- **Mean Squared Error**: 0.5417
- **R² Score**: 0.8992

### 3. Lasso Regression
- **Mean Absolute Error**: 1.2874
- **Mean Squared Error**: 0.5743
- **R² Score**: 0.8857

### 4. Random Forest Regression
- **Mean Absolute Error**: 0.9237
- **Mean Squared Error**: 0.3204
- **R² Score**: 0.9458

## Feature Importance (Random Forest)
The most influential features in predicting total orders are:
1. **total_sessions**: Importance 0.6754
2. **avg_rating**: Importance 0.1976
3. **avg_duration**: Importance 0.0931

## Recommendations
1. Focus on increasing user engagement by boosting cooking sessions, as it is the most predictive factor for orders.
2. Optimize platform features to cater to users with higher average session ratings.
3. Target marketing efforts towards dinner time to maximize order volumes.
4. Use Random Forest predictions for further marketing insights, given its high performance and feature interpretability.


### Visualizations:
- Top 10 Popular Dishes
- Cooking Sessions vs Orders
- Demographic Analysis: Favorite Meals by Location and Age
- Time of Day vs Total Orders
- Session Ratings vs Total Orders
"""
