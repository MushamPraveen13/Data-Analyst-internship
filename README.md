# Customer Lifetime Value (LTV) Prediction Model (REDAME )

## Project Overview
This project aims to predict the Lifetime Value (LTV) of customers by analyzing their purchase behavior. The predicted LTV helps businesses identify high-value customers, optimize marketing strategies, and improve retention efforts to drive sustainable growth.

## Key Objectives
- Analyze customer purchase history and engineer meaningful features (Recency, Frequency, Average Order Value).  
- Build and evaluate regression models (XGBoost, Random Forest) to predict LTV.  
- Segment customers based on predicted LTV for targeted marketing.  
- Deliver actionable insights through visualizations and model interpretability.

## Dataset
- *customers.xlsx*: Customer demographic and ID information.  
- *transactions.xlsx*: Historical transaction data including purchase amounts and dates.  

## Tools & Technologies

| Technology       | Purpose                                 |
|------------------|-----------------------------------------|
| Python           | Data processing, modeling               |
| pandas, numpy    | Data manipulation and feature engineering |
| scikit-learn     | Model building and evaluation           |
| XGBoost          | Gradient boosting regression            |
| joblib           | Model serialization                     |
| matplotlib, seaborn | Visualization                        |
| Excel            | Data storage and preprocessing          |

## Methodology

### Data Preprocessing
- Merged customer and transaction datasets.  
- Handled missing values and removed duplicates.  
- Converted date columns into usable formats.

### Feature Engineering
- Recency: Days since last purchase.  
- Frequency: Total number of purchases.  
- Average Order Value (AOV): Average purchase amount.

### Modeling
- Split data into training and testing sets.  
- Trained XGBoost and Random Forest regression models.  
- Evaluated model performance with MAE and RMSE.  
- Selected the best-performing model (XGBoost).

### Customer Segmentation
- Divided customers into four LTV segments (Very High, High, Medium, Low) based on quartiles of predicted LTV.

## Deliverables
- ltv_prediction_project.ipynb — Jupyter Notebook containing the entire analysis, modeling, and visualization pipeline.  
- ltv_model.pkl — Serialized trained model for future prediction.  
- ltv_predictions.csv — Customer IDs with predicted LTV and assigned segments.  
- Input datasets: customers.xlsx, transactions.xlsx  
- README.md — Project documentation.

## How to Run
1. Clone the repository.  
2. Install required packages:  
   ```bash
   pip install pandas numpy scikit-learn xgboost matplotlib seaborn joblib
