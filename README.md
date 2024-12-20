# Walmart-Sales-Forecasting <br>
This dataset focuses on predicting weekly store sales at Walmart by examining holiday effects, temporal patterns, and other influential factors. The goal is to enable efficient stock planning, revenue calculations, and strategic decision-making by understanding patterns related to seasonal sales fluctuations. <br>
This machine learning model is developed based on resources from : https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/overview/evaluation <br>

**Dataset Overview :** <br>
1. Test Data Contains 115,064 rows with information: Store, Department, Date, IsHoliday. "IsHoliday" indicates whether the week includes a special holiday. Holidays tend to show higher average sales than non-holiday periods. <br>
2. Train Data Also contains 115,064 rows with Store, Department, Date, IsHoliday, Weekly Sales. Weekly sales are the recorded weekly sales for specific departments at certain stores. <br>
3. Features Data Consists of 8,190 rows with variables such as Temperature, Fuel Price, CPI, Unemployment, Markdown 1-5, IsHoliday <br>
4. Store Data Includes details about Walmart stores such as store numbers, store types, and store sizes. <br>

The goal is to predict the impact of holidays on weekly store sales. To achieve this, a Time Series modeling approach was applied using variables such as date, weekly sales, is holiday, lag features, rolling averages, and XGBoost. The evaluation metric used was Weighted Mean Absolute Error (WMAE), which emphasizes periods of higher significance, such as holidays. <br>

**Final Model Metrics:** <br>
Weighted Mean Absolute Error = 211 <br>
Error rate relative to average weekly sales = ~1.32%. <br>
The low error percentage highlights the model's accuracy in forecasting weekly sales and assessing seasonal fluctuations.
