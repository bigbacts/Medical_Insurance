# Medical Insurance Cost Prediction

## Project Overview

This project focuses on the prediction of medical insurance charges using various machine learning techniques. The objective is to accurately estimate individual insurance costs based on demographic and lifestyle factors, including age, sex, BMI, number of children, smoking status, and region of residence.

## Dataset

- **Source:** [Kaggle Medical Cost Personal Dataset](https://www.kaggle.com/mirichoi0218/insurance) (or specify your dataset’s source if different)
- **Features:**
  - `age`: Age of the primary beneficiary
  - `sex`: Gender of the insurance contractor
  - `bmi`: Body mass index
  - `children`: Number of dependents covered by health insurance
  - `smoker`: Smoking status (yes/no)
  - `region`: Residential area in the United States
  - `charges`: Individual medical costs billed by health insurance

## Workflow

1. **Exploratory Data Analysis (EDA)**
   - Visualization and statistical analysis to identify key patterns and relationships among features.
2. **Feature Engineering**
   - One-hot encoding for categorical variables
   - Creation of interaction terms (such as age × BMI and smoker × BMI)
   - Log-transformation of the target variable to address skewness and improve model performance
3. **Model Development**
   - Linear Regression (including both standard and log-transformed target)
   - Decision Tree Regression
   - Random Forest Regression with hyperparameter tuning
   - Gradient Boosting Regression with hyperparameter tuning
   - Evaluation using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), R², and cross-validation for model robustness
4. **Model Interpretation**
   - Analysis of feature importance for tree-based models
   - Partial dependence plots to visualize feature impact
   - Residual plots to assess model diagnostics

## Key Findings

- Tree-based models (Random Forest and Gradient Boosting) outperformed linear models, achieving higher predictive accuracy and lower error rates.
- Smoking status, BMI, and age were identified as the most significant predictors of insurance charges.
- Log-transforming the target variable improved the performance of linear regression models by addressing right-skewed distribution.
- Cross-validation demonstrated the robustness and stability of the selected models.
- Feature engineering, including interaction terms, contributed marginal but measurable improvements in predictive performance.

## Conclusion

The analysis indicates that ensemble machine learning methods, particularly Random Forest and Gradient Boosting, provide the most accurate predictions for medical insurance costs when using this dataset. The project highlights the importance of smoking status, BMI, and age in influencing insurance charges, as well as the benefits of feature engineering and robust model evaluation.

## How to Run

1. Clone this repository.
2. Ensure the required Python libraries are installed (`requirements.txt` may be provided).
3. Run the Jupyter Notebook (`.ipynb` file) in your local environment or in a suitable cloud environment (such as Google Colab or Kaggle Kernels).

## License

Specify your project’s license here (e.g., MIT License).

## Contact

For questions or collaboration, please contact [Your Name] at [your-email@example.com].

