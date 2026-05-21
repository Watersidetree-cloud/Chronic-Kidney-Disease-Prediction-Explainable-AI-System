# Chronic Kidney Disease Prediction & Explainable AI System

> Built by Waterside Tree 🚀

## Project Overview

This project focuses on building an Explainable AI system capable of detecting the risk of Chronic Kidney Disease (CKD) using Machine Learning and clinical health indicators.

The system was designed not only to predict kidney disease risk but also to explain **why** a patient may be classified as high-risk or low-risk using SHAP Explainability techniques.

The project combines:

- Predictive Analytics
- Healthcare Intelligence
- Explainable AI (XAI)
- ML Experiment Tracking
- Model Interpretability

using Python, XGBoost, SHAP, MLflow, and Databricks.

---

# Business Problem

Chronic Kidney Disease is a major global healthcare challenge that often progresses silently until reaching severe stages.

Early detection can significantly improve:

- Treatment outcomes
- Risk management
- Clinical intervention
- Patient survival rates

Traditional diagnosis methods rely heavily on medical expertise and multiple clinical indicators. This project explores how Machine Learning can support healthcare professionals by identifying disease risk patterns from patient medical data.

The goal was to build a system capable of:

- Predicting CKD risk
- Identifying the most influential clinical indicators
- Explaining model predictions transparently

---

# Dataset Overview

The dataset contains:

- 1,659 patient records
- 52 medical and lifestyle-related features
- Binary diagnosis target variable

Some important features include:

- Serum Creatinine
- GFR (Glomerular Filtration Rate)
- HbA1c
- Protein in Urine
- Blood Pressure
- Hemoglobin Levels
- Cholesterol Levels
- Lifestyle & Behavioral Indicators

The project involved:

- Preprocessing
- Feature transformation
- Imbalance handling
- Model evaluation
- Explainability analysis

using Scikit-Learn pipelines and Databricks workflows.

---

# Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- SHAP
- MLflow
- Databricks
- Matplotlib
- Seaborn

---

# Machine Learning Workflow

## 1. Data Preprocessing

- Missing value handling
- Feature scaling
- Encoding categorical variables
- Column transformation pipelines

## 2. Class Balancing

RandomUnderSampler was used to handle class imbalance before model training.

## 3. Model Training

Three different machine learning models were trained and evaluated:

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

## 4. MLflow Experiment Tracking

MLflow was integrated for:

- Experiment logging
- Model tracking
- Parameter monitoring
- Metric evaluation
- Reproducibility

---

# Model Performance

## Logistic Regression

- F1 Score: 0.56
- Accuracy: 56%

## Random Forest

- F1 Score: 0.78
- Accuracy: 78%

## XGBoost (Best Model)

- F1 Score: 0.78
- Accuracy: 76%
- ROC-AUC Score: 0.79

The XGBoost model demonstrated the strongest balance between precision and recall for CKD prediction.

---

# Explainable AI (SHAP Analysis)

One of the most important parts of this project was model explainability.

SHAP (SHapley Additive exPlanations) was used to:

- Understand feature importance
- Explain prediction behavior
- Interpret patient-level predictions
- Increase healthcare transparency

## Most Influential Features

The model identified the following clinical indicators as the strongest drivers of CKD prediction:

- Serum Creatinine
- GFR
- Itching
- BMI
- Hemoglobin Levels
- HDL Cholesterol
- Systolic Blood Pressure
- Protein in Urine
- HbA1c
- BUN Levels

SHAP analysis revealed that kidney-function-related biomarkers played a major role in model decisions.

---

# Key Insights

## Serum Creatinine

The strongest predictor in the model.

Higher serum creatinine levels are commonly associated with impaired kidney filtration and reduced kidney function.

## GFR (Glomerular Filtration Rate)

Low GFR values strongly increased predicted CKD risk because GFR directly measures kidney efficiency.

## Protein in Urine

Protein leakage in urine became a major predictive signal because it often indicates kidney damage.

## HbA1c & Blood Sugar

Elevated HbA1c and fasting blood sugar levels contributed significantly to disease risk predictions due to their relationship with diabetes-related kidney damage.

---

# Explainable AI at Individual Patient Level

SHAP waterfall analysis was also used to explain predictions for individual patients.

This allowed the system to show:

- Which clinical indicators increased risk
- Which indicators reduced risk
- How different medical signals combined to influence final predictions

This creates a more transparent and interpretable healthcare AI system that healthcare professionals can better understand and trust.

---

# ROC Curve Evaluation

The XGBoost model achieved an ROC-AUC score of approximately 0.79, demonstrating strong ability to distinguish between CKD-positive and non-CKD patients.

This indicates the model learned clinically meaningful prediction patterns from the dataset.

---


# Future Improvements

Potential future improvements include:

- Hyperparameter optimization
- Deployment using FastAPI or Streamlit
- Real-time healthcare prediction APIs
- Deep Learning experimentation
- Integration with healthcare dashboards
- Model monitoring pipelines
- Clinical decision support integration

---

# Conclusion

This project demonstrates how Machine Learning and Explainable AI can be applied to healthcare risk prediction while maintaining transparency and interpretability.

Rather than focusing only on prediction accuracy, the project emphasizes the importance of building AI systems that healthcare professionals can understand, validate, and trust.

The future of healthcare AI will depend not only on intelligent models, but on interpretable systems capable of supporting real clinical decision-making.

---

# Author

**Tolulope Emuleomo**  
Data Scientist | Analytics Specialist

Company GitHub:  
https://github.com/Watersidetree-cloud

---

# Tags

`#HealthcareAI` `#ExplainableAI` `#MachineLearning` `#XGBoost` `#SHAP` `#Databricks` `#MLflow` `#Python` `#DataScience` `#HealthcareAnalytics` `#NaijaDataProfessor`
