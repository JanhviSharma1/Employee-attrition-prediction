# Employee Attrition Prediction

This project aims to predict whether an employee will leave the organization using historical HR data. The goal is to support HR departments in identifying high-risk employees and improving retention strategies.


## Dataset

- **Source**: IBM HR Analytics Employee Attrition & Performance dataset
- **Features**: 35 attributes including Age, JobRole, OverTime, MonthlyIncome, etc.
- **Target Variable**: `Attrition` (Yes/No)


## Tools & Technologies Used

- **Python** – Programming and analysis
- **Pandas** – Data handling and cleaning
- **Scikit-learn** – Model training, evaluation, preprocessing
- **Matplotlib & Seaborn** – Data visualization
- **Joblib & Pickle** – Model serialization
- **Jupyter Notebook / Python Script** – Development environment


## Workflow

1. **Data Preprocessing**
   - Removed irrelevant columns
   - Encoded categorical variables
   - Standardized numerical features

2. **Model Training**
   - Trained Logistic Regression and Random Forest models
   - Random Forest used for feature importance analysis

3. **Evaluation**
   - Logistic Regression Accuracy: **89.5%**
   - Random Forest Accuracy: **88.1%**
   - Used `classification_report` and `confusion_matrix` for model evaluation

4. **Model Serialization**
   - Saved final model and scaler using both `joblib` and `pickle` for future use


## Key Insights

- Top predictors of attrition include:
  - **OverTime**
  - **MonthlyIncome**
  - **JobRole**
  - **YearsAtCompany**
- Logistic Regression provided the best balance between accuracy and interpretability.

