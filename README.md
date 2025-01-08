# Smart Watch Data Analysis

## Objective and Scope
**Objective**: The goal of this project is to analyze smartwatch data to predict activity types and calories burned using various machine learning models. The specific objectives are:
- To understand the relationship between different features (steps, distance, heart rate, etc.) and the target variables (activity type and calories burned).
- To develop and evaluate machine learning models to accurately predict activity types and calories burned.
- To provide actionable insights and recommendations based on the analysis.

**Scope**: The scope of the analysis includes:
- Exploratory Data Analysis (EDA) to understand the data distribution, detect any anomalies, and explore relationships between features.
- Preprocessing steps such as handling missing values, encoding categorical variables, and feature scaling.
- Development of machine learning models, including Random Forest Classifier for activity type prediction and Stacking Regressor for calorie prediction.
- Evaluation of model performance using appropriate metrics.
- Generation of insights and recommendations based on the analysis results.

## Methodology
**Data Preprocessing**:
- Data Cleaning: Removed leading/trailing whitespace from column names and handled missing values using forward fill.
- Encoding Categorical Variables: Applied one-hot encoding to categorical features and label encoding to the target variable 'activity'.
- Feature Scaling: Normalized numeric features to ensure all features contribute equally to the model.

**Model Development**:
- Activity Type Prediction: Used a Random Forest Classifier to predict activity types. The model was trained and evaluated using accuracy, precision, recall, and F1-score.
- Calorie Prediction: Used a Stacking Regressor combining Linear Regression, Decision Tree Regressor, and Random Forest Regressor as base models, with Random Forest Regressor as the meta-model. The model was evaluated using Mean Squared Error (MSE) and R-squared (R²).

## Results and Insights
- **Random Forest Classifier**:
  - Initial Accuracy: 86.81%
  - Improved Accuracy after tuning: 86.97%
  - Classification Report indicated balanced precision and recall across activity types.

- **Stacking Regressor**:
  - Mean Squared Error (MSE): [Insert MSE value]
  - R-squared (R²): [Insert R² value]
  - Predicted Calories Burned showed consistent and accurate predictions.

## Recommendations
- For Users: Monitor and track steps, distance, and heart rate to optimize health and fitness activities.
- For Developers: Enhance smartwatch sensors for more accurate data collection.
- For Health Practitioners: Use smartwatch data insights to provide personalized health advice to users.

## Final Report
- Key Findings: Machine learning models, including Random Forest Classifier and Stacking Regressor, were effective in predicting activity types and calories burned.
- Visuals: Include visualizations such as correlation heatmaps, distribution plots, and model performance charts to support the findings.
- Limitations: The analysis assumed that the data was accurately recorded by the smartwatch sensors. Any sensor errors could affect the model's accuracy. The dataset's diversity in terms of user demographics and activity types was not considered, which might limit the model's generalizability.
- Potential for Further Exploration: Further exploration could involve incorporating more features, such as sleep patterns and diet data, to enhance prediction accuracy. Investigate the impact of different machine learning algorithms and hyperparameter tuning to improve model performance.
