# Guvi Project_4
## Dominos - Predictive Purchase Order System

### INTRODUCTION
Managing inventory efficiently is a challenge in the food service industry, where overstocking leads to waste and understocking results in lost sales. This project uses machine learning to predict pizza sales and generate an optimized purchase order for ingredients. By automating inventory management, this system helps Domino’s reduce costs, prevent stock shortages, and improve operational efficiency.

### PROJECT OVERVIEW
The goal of this project is to forecast pizza sales for the next 7 days and calculate the required ingredient quantities based on predicted demand. By leveraging historical sales data, the system ensures accurate inventory planning, reducing waste and improving supply chain management.

### KEY FEATURES
1. **Data Preprocessing:** Cleaned missing values, handled outliers, and created time-based features.
2. **Sales Forecasting:** Evaluated six machine learning models for demand prediction.
3. **Model Comparison:** Selected XGBoost as the best model based on Mean Absolute Percentage Error (MAPE).
4. **Automated Purchase Order:** Mapped predicted sales to ingredient usage data to generate purchase orders.
5. **Business Optimization:** Reduced manual effort in inventory planning, minimizing costs and stockouts.

### DATASET OVERVIEW
This project uses two datasets:
1. **Sales Data:** Historical pizza sales records, including order_date, pizza_name_id, and quantity_sold.
2. **Ingredient Data:** Defines ingredient requirements per pizza type, including pizza_ingredients and Items_Qty_In_Grams.

### MODEL PERFORMANCE (MAPE Scores - Lower is Better)
1. **ARIMA** – Moderate error, struggled with trend shifts.
2. **SARIMA** – Improved over ARIMA but less accurate than tree-based models.
3. **Prophet** – Performed well but sensitive to missing data.
4. **Linear Regression** – High error, unable to capture non-linear trends.
5. **Random Forest** – Good accuracy but prone to overfitting.
6. **XGBoost** – Best performance, lowest MAPE score, selected for final predictions.

### CONCLUSION
This project successfully demonstrates how machine learning can optimize inventory management in the food industry. The XGBoost model provided accurate sales forecasts, enabling automated purchase order generation. This system helps Domino’s minimize waste, reduce costs, and ensure seamless kitchen operations. Future improvements could include real-time inventory tracking and seasonal trend analysis to further enhance accuracy and efficiency. 
