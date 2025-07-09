# Case Study: Restaurant Sales Forecasting & Analysis
Objective:-
This project aimed to analyze restaurant sales data across multiple stores and forecast future performance using both traditional machine learning and deep learning models. As an aspiring data analyst, the focus was on uncovering insights, identifying trends, and delivering business value through data-driven decisions.

Dataset Summary:-
Combined multiple datasets including sales records, product info, and store details
Final dataset included:
date, item_id, item_name, price, item_count
kcal (calories), store_id, store_name
Cleaned and merged into a structured format for analysis

Exploratory Data Analysis (EDA):-
I focused on drawing actionable insights through:
Time-Based Analysis:
-Identified trends in daily, monthly, and quarterly sales
-Analyzed day-of-week patterns to understand customer behavior
-Detected seasonal peaks and dips in performance
Store-Wise Performance:
-Compared total sales across different restaurants
-Tracked individual store trends by year, month, and day
-Identified the top-performing and underperforming stores
Product-Level Insights:
-Determined best-selling items and where they were sold
-Found the most popular item at each store
-Analyzed the relationship between item popularity, price, and calories
-Identified the most expensive item at each store and checked calorie content
Revenue vs. Volume:
-Compared daily sales volume and revenue to find if the highest-selling store also earned the most

Feature Engineering:-
Generated several new features to support analysis and modeling:
-day_of_week, month, year, quarter, day_of_month
-Lag features for sales prediction
-Aggregated KPIs for modeling and visualizations

Machine Learning Models:-
-Built and compared the performance of 3 models to forecast item count:
   -linear Regression
   -Random Forest
   -XGBoost
-Used the last 6 months of data as a test set
-Computed RMSE for model comparison
-Selected the best-performing model to forecast the next year’s item counts

Deep Learning Forecasting (LSTM):-
Applied an LSTM (Long Short-Term Memory) neural network to predict sales amount rather than item count:
-Preprocessed the data for sequence learning
-Defined time series windows for training/testing
-Trained the model on historical sales data
-Evaluated performance using Mean Absolute Percentage Error (MAPE)
Built a second LSTM model trained on the entire series to forecast the next 3 months

Key Insights:-
-Weekends (especially Sundays) consistently saw higher sales across stores
-Store performance varied significantly by region and season
-Some stores had high volume but lower revenue due to low-price items
-Certain high-priced, high-calorie items were top-sellers at specific stores — useful for targeted promotions
-XGBoost outperformed other ML models on test RMSE
-LSTM produced reliable short-term forecasts with acceptable MAPE

Tools & Libraries Used:-
-Python: Core language for data manipulation and modeling
-Pandas, NumPy: Data cleaning, wrangling, and transformation
-Matplotlib, Seaborn: Visualizations and charts
-Scikit-learn: ML models and evaluation
-XGBoost: Advanced ensemble modeling
-TensorFlow / Keras: LSTM neural network
-Google Colab: Cloud-based notebook environment
