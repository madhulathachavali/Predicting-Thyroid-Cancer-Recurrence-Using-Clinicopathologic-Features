# Predicting-Thyroid-Cancer-Recurrence-Using-Clinicopathologic-Features

### Objective:
The primary goal of this analysis is to **predict the recurrence** of well-differentiated thyroid cancer based on the provided clinicopathologic features.

---

### Dataset Overview
This dataset, "**Differentiated Thyroid Cancer Recurrence**," was compiled by **Borzooei, S. & Tarokhian, A. (2023)** and is available through the **[UCI Machine Learning Repository](https://doi.org/10.24432/C5632J)**. It contains **13 clinicopathologic features** collected over **15 years** to predict the recurrence of well-differentiated thyroid cancer (WDTC). The dataset includes data from patients who were followed for at least **10 years**. 

**Reference:**  
Borzooei, S. & Tarokhian, A. (2023). Differentiated Thyroid Cancer Recurrence [Dataset]. UCI Machine Learning Repository. [DOI: 10.24432/C5632J](https://doi.org/10.24432/C5632J).

---

### Dataset Features
The dataset includes the following features:

- **Age**: Age of the patient at the time of diagnosis (Real).
- **Gender**: Patient's gender (Categorical: Male/Female).
- **Smoking**: Whether the patient smoked or not (Categorical: Yes/No).
- **Hx Smoking**: History of smoking (Categorical: Yes/No).
- **Hx Radiotherapy**: Whether the patient had prior radiotherapy (Categorical: Yes/No).
- **Thyroid Function**: Functioning of the thyroid (Real).
- **Physical Examination**: Clinical findings from physical exams (Categorical).
- **Adenopathy**: Presence of lymph node enlargement (Categorical: Yes/No).
- **Pathology**: Histopathological findings (Categorical).
- **Focality**: Whether the tumor is focal or multifocal (Categorical).
- **Risk**: Risk level for cancer recurrence (Integer).
- **T (Tumor Size/Extent)**: Tumor size or extent of local invasion (Categorical: T1, T2, T3, T4).
- **N (Lymph Node Involvement)**: Lymph node involvement (Categorical: N0, N1a, N1b).
- **M (Metastasis)**: Distant metastasis (Categorical: M0, M1).
- **Stage**: The cancer stage, based on the TNM classification (Integer).
- **Response**: Response to initial treatment (Integer: 0 = No Response, 1 = Partial Response, 2 = Complete Response).
- **Recurred**: Whether the cancer recurred (Target variable: 0 = No, 1 = Yes).

---

### Data Summary


| Variable             | Mean ± Std                                                                                                                                | Min   | Max   | Median   |
|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------|-------|-------|----------|
| Age                  | 40.87 ± 15.13                                                                                                                             | 15    | 82    | 37.0     |
| Gender               | F: 312, M: 71                                                                                                                             | -     | -     | -        |
| Smoking              | No: 334, Yes: 49                                                                                                                          | -     | -     | -        |
| Hx Smoking           | No: 355, Yes: 28                                                                                                                          | -     | -     | -        |
| Physical Examination | Multinodular goiter: 140, Single nodular goiter-right: 140, Single nodular goiter-left: 89, Normal: 7, Diffuse goiter: 7                  | -     | -     | -        |
| Thyroid Function     | Euthyroid: 332, Clinical Hyperthyroidism: 20, Subclinical Hypothyroidism: 14, Clinical Hypothyroidism: 12, Subclinical Hyperthyroidism: 5 | -     | -     | -        |
| Adenopathy           | No: 277, Right: 48, Bilateral: 32, Left: 17, Extensive: 7, Posterior: 2                                                                   | -     | -     | -        |
| Pathology            | Papillary: 287, Micropapillary: 48, Follicular: 28, Hurthel cell: 20                                                                      | -     | -     | -        |
| Focality             | Uni-Focal: 247, Multi-Focal: 136                                                                                                          | -     | -     | -        |
| Risk                 | Low: 249, Intermediate: 102, High: 32                                                                                                     | -     | -     | -        |
| T                    | T2: 151, T3a: 96, T1a: 49, T1b: 43, T4a: 20, T3b: 16, T4b: 8                                                                              | -     | -     | -        |
| N                    | N0: 268, N1b: 93, N1a: 22                                                                                                                 | -     | -     | -        |
| M                    | M0: 365, M1: 18                                                                                                                           | -     | -     | -        |
| Stage                | I: 333, II: 32, IVB: 11, III: 4, IVA: 3                                                                                                   | -     | -     | -        |
| Response             | Excellent: 208, Structural Incomplete: 91, Indeterminate: 61, Biochemical Incomplete: 23                                                  | -     | -     | -        |
| Recurred             | No: 275, Yes: 108                                                                                                                         | -     | -     | -        |

<img width="798" alt="image" src="https://github.com/user-attachments/assets/55b7de78-5d60-49ff-aef6-fbff7a387e82" />


---

## Model Performance
The three machine learning models—Logistic Regression, Support Vector Machine (SVM), and Decision Tree Classifier were evaluated for predicting the recurrence of well-differentiated thyroid cancer, based on the following features: Age, Smoking, Hx Radiotherapy, N (Lymph Node Involvement), T (Tumor Size/Stage), M (Metastasis), Stage (Cancer Stage) and Response (Response to treatment). 

### Model Comparison: Logistic Regression, SVM, and Decision Tree Classifier

| **Model**              | **Accuracy** | **Precision** | **Recall**  | **F1-Score** | **Macro Avg** | **Weighted Avg** |
|------------------------|--------------|---------------|-------------|--------------|---------------|------------------|
| **Logistic Regression** | 93.04%       | 92.97%        | 93.04%      | 92.97%       | 91.17%        | 92.97%           |
| **SVM**                 | 96.52%       | 97.59%        | 93.75%      | 96.52%       | 95.67%        | 96.52%           |
| **Decision Tree**       | 92.17%       | 94.55%        | 86.15%      | 92.21%       | 90.35%        | 92.21%           |

- **SVM** performed the best across all evaluation metrics: accuracy, precision, recall, and F1-score.












