# Medical Insurance Cost Prediction

This project aims to predict the medical insurance cost for individuals using machine learning models. The dataset used in this project is based on the "Machine Learning with R" book by Brett Lantz and has been cleaned and prepared for analysis.

The dataset comes from Kaggle - https://www.kaggle.com/datasets/mirichoi0218/insurance

## Dataset

The dataset contains the following columns:

- `age`: Age of the primary beneficiary
- `sex`: Insurance contractor gender (female, male)
- `bmi`: Body mass index, providing an understanding of body weights that are relatively high or low relative to height (kg / m ^ 2)
- `children`: Number of children covered by health insurance / Number of dependents
- `smoker`: Smoking status (yes, no)
- `region`: The beneficiary's residential area in the US (northeast, southeast, southwest, northwest)
- `charges`: Individual medical costs billed by health insurance

## Exploratory Data Analysis

The project begins with exploratory data analysis to understand the data and its distribution. Various visualizations are used to analyze the relationship between the target variable (charges) and the other features.

- A histogram is plotted to visualize the distribution of medical costs.
- A heatmap is created to display the correlation between features.

## Feature Engineering

Before training the machine learning models, some preprocessing is performed:

- Label encoding is applied to convert categorical variables (`sex`, `smoker`, and `region`) into numerical representations.
- BMI values are categorized into four groups (underweight, normal weight, overweight, and obesity) based on standard BMI ranges.

## Machine Learning Models

Several regression models are trained to predict the medical insurance cost:

- Linear Regression
- Lasso Regression
- Ridge Regression
- ElasticNet Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor

## Model Evaluation

The models are evaluated using cross-validation techniques. Performance metrics like Root Mean Squared Error (RMSE) and R-squared (R2) are used to compare and select the best-performing models.

## Hyperparameter Tuning

The best-performing models are further fine-tuned using GridSearchCV to optimize their hyperparameters. This process involves systematically exploring a range of hyperparameter values to find the best combination that improves the model's performance.

## Feature Importance

Feature importance is analyzed to identify the most significant features that influence medical insurance costs. Visualizations such as bar plots and decision tree plots are used to understand the importance of each feature.

## Conclusion

Based on the evaluation results, the best-performing model and its hyperparameters are selected for predicting medical insurance costs. The model can be used to make predictions for individuals and help insurers in cost estimation and decision-making processes.

## Additional Information

I originally wrote the code for a group project during the Data Science Bootcamp at infoShare Academy.

Overall, the modified code is more organized, better documented, and incorporates better data preprocessing, hyperparameter tuning, and model evaluation techniques. It is easier to understand and maintain, and provides a more comprehensive analysis of the data and models.