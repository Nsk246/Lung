# Lung Cancer Survival Prediction

This project builds a predictive model to determine whether a lung cancer patient is likely to survive, based on diagnostic and personal data. This can assist healthcare professionals in identifying high-risk cases and optimizing treatment plans.

---

## Objective

To predict patient survival using machine learning models based on diagnostic data, aiming to improve decision-making in lung cancer treatment.

---

## Dataset

The dataset contains comprehensive patient information, focused on lung cancer diagnostics and outcomes.

### Features

- **Age**: The age at the time of diagnosis or treatment.
- **Gender**: The gender of the patient (male or female).
- **Smoking**: Whether the patient is a smoker or not.
- **Hx Smoking**: Smoking history of the patient (e.g., whether they have ever smoked).
- **Hx Radiotherapy**: History of radiotherapy treatment for any condition.
- **Thyroid Function**: The status of thyroid function, possibly indicating abnormalities.
- **Physical Examination**: Findings from a physical examination of the patient.
- **Adenopathy**: Presence or absence of enlarged lymph nodes (adenopathy) in the neck region.
- **Pathology**: Specific type of thyroid cancer determined by pathological examination.
- **Focality**: Whether the cancer is unifocal (limited to one location) or multifocal (present in multiple locations).
- **Risk**: The risk category of the cancer based on tumor size, spread extent, and histological type.
- **T**: Tumor classification based on size and extent of invasion into nearby structures.
- **N**: Nodal classification indicating lymph node involvement.
- **M**: Metastasis classification indicating distant metastases presence or absence.
- **Stage**: The overall stage of the cancer, typically determined by combining T, N, and M classifications.
- **Response**: Response to treatment, indicating whether the cancer responded positively, negatively, or remained stable after treatment.
- **Recurred**: Indicates whether the cancer recurred after initial treatment.

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

