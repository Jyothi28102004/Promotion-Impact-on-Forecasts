# Promotion-Impact-on-Forecasts
"Real-time sales forecasting project analyzing promotion impact using XGBoost"

📈 Promotion Impact on Forecasts
A real-time, end-to-end data science project that evaluates how promotions affect retail sales forecasts. Built using Python, XGBoost, and optional Power BI, this project compares sales uplift when promotion campaigns are included in forecasting models — enabling data-driven marketing and inventory planning.

📌 Objective
To build forecasting models that help retailers:

Measure the real impact of discounts or promotions

Predict sales with and without promotional features

Evaluate whether promotions cause genuine uplift or short-term shifts

Enable strategic decisions for campaign planning and profitability

🗃️ Dataset Description
Used a real-life retail dataset containing multiple sheets (e.g., 2009-2010, 2010-2011) manually uploaded into Google Colab from an ERP-style reporting file.

Main columns:

Date: Transaction date

Item: Product description

Quantity: Units sold

Promotion: Custom binary column (1 = promo active, 0 = not)

(Optional) Store, Region, Category

✅ Dataset structure and format simulate real-time, production-style sales data extracted from Excel files.

🧠 Technologies & Tools
Python (Pandas, Numpy, Matplotlib, Seaborn)

XGBoost Regressor (main forecasting model)

scikit-learn (metrics and train-test split)

Google Colab (development environment)

Power BI (optional visualization dashboard)

GitHub (version control and deployment)

🧪 Project Phases
✅ Phase 1: Data Preparation & Cleaning
Manually uploaded Excel file with multiple sheets

Read and combined 2009-2010, 2010-2011 into a single DataFrame

Handled null values, removed duplicates, standardized column names

Created Promotion binary variable

Parsed dates and extracted time components (year, month, weekday)

✅ Phase 2: Exploratory Data Analysis (EDA)
Analyzed sales trends over months and years

Visualized distribution of sales with/without promotions

Correlation between promotions and quantity sold

Countplots and boxplots for promotional activity

✅ Phase 3: Feature Engineering
Extracted time-based features: Month, Year, Weekday

Created lag features and rolling averages of quantity

Encoded categorical variables (optional)

Constructed Promotion as a key forecasting input

✅ Phase 4: Forecasting with XGBoost
Time-based train-test split (train: before promo, test: after)

Trained XGBoostRegressor with and without Promotion as input

Tuned parameters for tree depth, learning rate, and early stopping

Generated predictions and saved to CSV

✅ Phase 5: Evaluation & Uplift Analysis
Compared model performance (MAE, RMSE)

Visualized:

Actual vs Predicted Sales

Sales uplift caused by promotions

Computed uplift = (Pred_with_promo - Pred_without_promo)

📊 Visualizations
📈 Actual vs Predicted Sales Line Chart

📊 Sales Uplift Bar Plot

🔍 Distribution of sales during promotion vs non-promotion periods


🎯 Outcome
Delivered a quantitative framework to assess promotion impact

Helped identify whether campaigns drive true sales uplift or just shift demand

Simulated a production-grade pipeline for promotional forecasting

