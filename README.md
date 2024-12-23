


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

## Recommendations:
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
