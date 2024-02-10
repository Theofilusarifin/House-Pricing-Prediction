# House Pricing Prediction

## Introduction
Real Estate refers to tangible properties such as land, buildings, or other structures, which can serve as investment assets or a source of income through rent or property sales. Machine Learning plays a crucial role in the real estate industry by predicting property prices based on factors such as location, size, amenities, and property condition, assisting agents, investors, and sellers in determining the right price.

## Goals
The goal of this project is to build a machine learning model that can predict the selling prices of houses in the Ames area, Iowa, US.

[Documentation Details](https://github.com/Theofilusarifin/House-Pricing-Prediction/blob/main/documentation.pdf)

## Exploratory Data Analysis (EDA)
- **Dataset Overview:** The dataset contains X samples and Y features.
- **Data Cleaning:** Handled missing values and outliers.
- **Feature Engineering:** Created new features such as total square footage and price per square foot.
- **Visualization:** Explored the relationships between features and target variable using plots.

## Modeling
- **Model Selection:** Evaluated various regression models such as Linear Regression, Ridge Regression, Lasso Regression, and Gradient Boosting Regression.
- **Hyperparameter Tuning:** Tuned hyperparameters of the best model using grid search.
- **Evaluation Metrics:**
    - **Root Mean Squared Error (RMSE):** Measures the average error of the model's predictions.
    - **R-squared (R2):** Indicates the proportion of the variance in the dependent variable that is predictable from the independent variables.
    - **Mean Absolute Error (MAE):** Represents the average absolute difference between the predicted and actual values.
    - **Explained Variance Score:** Indicates the proportion of variance in the target variable that the model explains.
    - **Median Absolute Error (MedAE):** Represents the median absolute difference between the predicted and actual values.

### Model Performance
| Model                      | RMSE  | R2    | MAE   | Explained Variance Score | MedAE |
|----------------------------|-------|-------|-------|--------------------------|-------|
| SGDRegressor               | 0.109 | 0.929 | 0.074 | 0.936                    | 0.050 |
| GradientBoostingRegressor | 0.086 | 0.955 | 0.066 | 0.969                    | 0.052 |
| LinearRegression           | 0.106 | 0.933 | 0.072 | 0.939                    | 0.053 |
| Ridge                      | 0.107 | 0.932 | 0.072 | 0.938                    | 0.052 |
| **Best Model**             | **0.086** | **0.955** | **0.066** | **0.969** | **0.052** |

## Model Deployment
The best performing model has been deployed using Streamlit. You can access the deployed application [here](https://housing-price-prediction-alan-turing.streamlit.app/).

## Conclusion
The Gradient Boosting Regressor performed the best among the models evaluated, achieving an RMSE of 0.086 and R-squared of 0.955. Further improvements could be made by incorporating additional features or exploring different modeling techniques.
