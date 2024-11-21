# AIML CA1: Data Analysis and Machine Learning

This project comprises two parts, focusing on predictive modeling tasks related to water quality and hospital costs using machine learning techniques.

---

## Part A: Predicting Water Quality

### Objective
To determine how various water variables impact water quality and predict whether the quality is good or bad.

### Key Steps
1. **Dataset Overview**:
   - Used `CA1-Classification-Dataset.csv`, which includes multiple features related to water quality.
   - Handled missing data by imputing column means.

2. **Feature Engineering**:
   - Selected a **Decision Tree model** for initial testing.
   - Performed iterative feature removal and identified `Organic_carbon` as the least impactful feature, which was dropped.

3. **Model Selection**:
   - Decision Tree was chosen after testing and tuning other models, as it provided the best balance of performance for this task.

4. **Hyperparameter Tuning**:
   - Improved accuracy through tuning.
   - Observed increased precision but a decline in recall, F1 score, and AUC.

### Conclusion
The tuned model achieved higher accuracy, but trade-offs in other metrics highlight the need to balance precision and recall for optimal predictions.

---

## Part B: Predicting Hospital Costs

### Objective
To predict how various variables influence hospital costs for admitted patients.

### Key Steps
1. **Dataset Overview**:
   - Used `CA1-Regression-Dataset.csv`, containing variables like `age`, `gender`, `BMI`, `region`, and `smoker status`.
   - Applied **one-hot encoding** to convert categorical data to numeric format.
   - Set `hospital cost` as the target variable.

2. **Feature Processing**:
   - Identified and dropped the `region` variable due to its minimal importance.

3. **Model Selection**:
   - Chose **Random Forest Regressor** based on superior performance compared to other models.

4. **Hyperparameter Tuning**:
   - Adjusted parameters to improve model performance.

### Conclusion
The final model demonstrated reliable predictions, emphasizing the importance of feature selection and parameter tuning in regression tasks.

---

This project showcases the use of data preprocessing, feature engineering, and machine learning algorithms to solve classification and regression problems effectively.

