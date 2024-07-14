# Customer Lifetime Value Prediction

This repository contains code and resources for predicting Customer Lifetime Value (CLV) in the insurance industry using machine learning techniques. CLV is a crucial metric that helps businesses understand the value a customer brings over their relationship with the company, guiding decisions on marketing strategies, customer retention efforts, and overall profitability.

## Dataset

The dataset used includes a variety of customer attributes such as Vehicle Class, Coverage type, Renew Offer Type, Employment Status, Marital Status, Education level, Number of Policies, Monthly Premium Auto, Total Claim Amount, Income, and the target variable Customer Lifetime Value (CLV).

## Models and Evaluation

Several machine learning models were evaluated to predict CLV:

- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **Random Forest**
- **XGBoost**

Evaluation metrics such as Mean Absolute Percentage Error (MAPE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²) were used to assess model performance. Based on these metrics, Random Forest emerged as the top-performing model with a MAPE of 4.815% and an R² of 0.904.

### Model Tuning

The Random Forest model was further optimized with the following parameters:
- `max_depth`: 10
- `min_samples_leaf`: 2
- `min_samples_split`: 5
- `n_estimators`: 100

### Interpretability with SHAP

To gain insights into feature importance and model predictions, SHAP (SHapley Additive exPlanations) was employed. This analysis highlighted features such as Monthly Premium Auto and Total Claim Amount as significant contributors to CLV predictions.

## Usage

To replicate the analysis:
1. Clone this repository.
2. Install the necessary dependencies as specified in `requirements.txt`.
3. Run the notebooks or scripts provided to train and evaluate the models.
4. Explore the SHAP outputs to understand feature contributions to predictions.

## Conclusion

The insights gained from this project can assist insurance companies in:
- Targeting marketing efforts more effectively.
- Improving customer retention strategies.
- Optimizing customer lifetime value across different segments.

## Requirement
- pip
- jupyter
- db-dtypes
- google-cloud-aiplatform
- google-cloud-bigquery
- google-cloud-storage
- google-auth
- scikit-learn==1.2.2
- setuptools==68.2.2
- numpy==1.26.4
- scipy==1.11.4
- pandas==2.1.4
- matplotlib==3.8.0
- joblib==1.2.0
- threadpoolctl==2.2.0
