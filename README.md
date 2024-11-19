# Lung Cancer Survival Prediction

This project builds a predictive model to determine whether a lung cancer patient is likely to survive, based on diagnostic and personal data. This can assist healthcare professionals in identifying high-risk cases and optimizing treatment plans.

---

## Objective

To predict patient survival using machine learning models based on diagnostic data, aiming to improve decision-making in lung cancer treatment.

---

## Dataset

The dataset contains comprehensive patient information focused on lung cancer diagnostics and outcomes.

### Features

- **id**: A unique identifier for each patient in the dataset.
- **age**: The age of the patient at the time of diagnosis.
- **gender**: The gender of the patient (e.g., male, female).
- **country**: The country or region where the patient resides.
- **diagnosis_date**: The date on which the patient was diagnosed with lung cancer.
- **cancer_stage**: The stage of lung cancer at the time of diagnosis (e.g., Stage I, Stage II, Stage III, Stage IV).
- **family_history**: Indicates whether there is a family history of cancer (e.g., yes, no).
- **smoking_status**: The smoking status of the patient (e.g., current smoker, former smoker, never smoked, passive smoker).
- **bmi**: The Body Mass Index of the patient at the time of diagnosis.
- **cholesterol_level**: The cholesterol level of the patient (value).
- **hypertension**: Indicates whether the patient has hypertension (e.g., yes, no).
- **asthma**: Indicates whether the patient has asthma (e.g., yes, no).
- **cirrhosis**: Indicates whether the patient has cirrhosis of the liver (e.g., yes, no).
- **other_cancer**: Indicates whether the patient has had any other type of cancer in addition to the primary diagnosis (e.g., yes, no).
- **treatment_type**: The type of treatment the patient received (e.g., surgery, chemotherapy, radiation, combined).
- **end_treatment_date**: The date on which the patient completed their cancer treatment or died.
- **survived**: Indicates whether the patient survived (e.g., yes, no).

---

## Models and Results

### 1. Random Forest Classifier

- **Accuracy**: 77.77%
- **Confusion Matrix**:
            precision    recall  f1-score   support

       0       0.78      1.00      0.87    138639
       1       0.24      0.00      0.00     39361

accuracy                           0.78    178000

---

### Insights

- The Random Forest model performs well on **class 0 (non-survived)** but struggles significantly with **class 1 (survived)**.
- The low recall for class 1 indicates the model fails to identify most patients who survived.

---

