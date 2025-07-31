  This study evaluated XGBoost, LightGBM, and Neural Networks for binary classification in a clinical dataset. Among the models, XGBoost performed best, achieving 90% accuracy and an ROC-AUC of 0.8997, indicating strong discriminative power. LightGBM followed closely with 89% accuracy, while the Neural Network lagged at 81%.
Age-group-specific analysis showed XGBoost consistently outperformed LightGBM, especially in the 31–50 and 51–70 age ranges, with ROC-AUC scores above 0.88. However, performance dropped for younger (0–30) groups due to limited positive samples, suggesting data imbalance as a challenge. SHAP analysis revealed Feature 2, Feature 8, and Feature 7 as the most influential, with Feature 2 showing the strongest impact on predictions. Some features (e.g., Feature 3, 10) had minimal influence and could be excluded in future iterations. Overall, XGBoost proved robust and generalizable, making it a reliable model for health outcome prediction. Future work could focus on addressing class imbalance, incorporating more relevant features, and exploring ensemble or deep learning improvements for enhanced performance and interpretability



**DATASET DESCRIPTION:**

The dataset used in this study is a comprehensive healthcare dataset sourced from a repository for stroke risk analysis. It contains 5,110 records and 12 attributes that span demographic, medical, and lifestyle factors. The primary focus of this project is to predict the risk of hypertension based on age and other influencing factors.

Key columns include:
Age (float): A continuous variable ranging from 0.08 to 82 years, which serves as the central feature in our age-wise hypertension analysis.

Hypertension (int): A binary variable indicating whether the individual has been diagnosed with hypertension (1) or not (0), used as the target variable.

Gender (object): Categorical, with values such as Male, Female, and Other.

Heart Disease (int): Indicates if the individual has a history of heart disease.

Ever Married (object): Reflects marital status, a possible sociodemographic determinant.

Work Type (object) and Residence Type (object): Represent the individual’s professional and residential environments, potentially affecting lifestyle and health.

Average Glucose Level (float) and BMI (float): Clinical indicators of metabolic health.
    Smoking Status (object): Categorical variable with four levels—‘never smoked’, ‘formerly smoked’, ‘smokes’, and ‘Unknown’.

The dataset has minimal missing data, with BMI missing in 201 entries. No other column contains missing values. The dataset is balanced enough to support various machine learning models. The presence of rich features makes it well-suited for predictive modeling of hypertension risk, especially in age-stratified analysis. 
