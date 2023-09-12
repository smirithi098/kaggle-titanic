# Titanic - Survival Prediction

Link to project: [Project on kaggle](https://www.kaggle.com/code/smirithi/survival-prediction)

The objective of the project was to use machine learning model to predict which passengers survived the titanic sinking given a number of parameters to identify them. The model's performance is evaludated using the metric **RMSE (Root Mean Squared Error)**.

### Data Preparation
On basic analysis of the data, the following steps were performed:
1. **Imputation**: *Age* being a continuous numeric feature, the missing values were replaced with the median. *Embarked*, a categorical feature, mode was used to replace the missing values.
2. **Removing columns**: Certain features with information irrelevant for the model training were dropped.
3. **Label encoding**: The data had 2 text features namely, *Sex* & *Embarked* which were label encoded to convert to numeric columns.

### Models Applied
For this project, I have used a *Pipeline* to include steps namely, 
- **Scaler** to standardize the column values to bring them to an equal scale
- **Variance Threshold** for feature engineering to remove features that have low variance
- **Grid Search** to find the best suitable parameters for the machine learning models to perform at their best

The following have applied to 2 classification models: *Support Vector Machine* & *Logistic Regression*

### Packages Used
- Pandas
- Numpy
- Sklearn
- Seaborn
