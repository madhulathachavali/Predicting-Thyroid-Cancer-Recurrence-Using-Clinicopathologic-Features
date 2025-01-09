# Predicting-Thyroid-Cancer-Recurrence-Using-Clinicopathologic-Features

The primary goal of this analysis is to predict recurrence of well-differentiated thyroid cancer based on the provided clinicopathologic features. 

Dataset Overview
This dataset, "Differentiated Thyroid Cancer Recurrence," was compiled by Borzooei, S. & Tarokhian, A. (2023) and is available through the UCI Machine Learning Repository here. It contains 13 clinicopathologic features collected over 15 years to predict the recurrence of well-differentiated thyroid cancer (WDTC). The dataset includes data from patients who were followed for at least 10 years. (Borzooei, S. & Tarokhian, A. (2023). Differentiated Thyroid Cancer Recurrence [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5632J.)

Dataset Features
The dataset includes the following features:

Age: Age of the patient at the time of diagnosis (Real).

Gender: Patient's gender (Categorical: Male/Female).

Smoking: Whether the patient smoked or not (Categorical: Yes/No).

Hx Smoking: History of smoking (Categorical: Yes/No).

Hx Radiotherapy: Whether the patient had prior radiotherapy (Categorical: Yes/No).

Thyroid Function: Functioning of the thyroid (Real).

Physical Examination: Clinical findings from physical exams (Categorical).

Adenopathy: Presence of lymph node enlargement (Categorical: Yes/No).

Pathology: Histopathological findings (Categorical).

Focality: Whether the tumor is focal or multifocal (Categorical).

Risk: Risk level for cancer recurrence (Integer).

T (Tumor Size/Extent): Tumor size or extent of local invasion (Categorical: T1, T2, T3, T4).

N (Lymph Node Involvement): Lymph node involvement (Categorical: N0, N1a, N1b).

M (Metastasis): Distant metastasis (Categorical: M0, M1).

Stage: The cancer stage, based on the TNM classification (Integer).

Response: Response to initial treatment (Integer: 0 = No Response, 1 = Partial Response, 2 = Complete Response).

Recurred: Whether the cancer recurred (Target variable: 0 = No, 1 = Yes).

## Descriptive Analysis

Age:

The dataset contains individuals aged from 15 to 82 years, with a mean age of 40.87 years and a standard deviation of 15.13 years. 

Gender:

The dataset includes 312 females (0) and 71 males (1), showing a higher representation of females.

T (Tumor Size):

T2 is the most common tumor size, followed by T3a and T1a. Larger tumor classifications (T3 and T4) are associated with a higher risk of recurrence.

N (Lymph Node Involvement):

N0 (no lymph node involvement) is the most frequent, while N1a and N1b indicate lymph node spread. Lymph node involvement significantly increases the risk of recurrence.

M (Metastasis):

M0 (no metastasis) is prevalent in the dataset, but M1 (distant metastasis) indicates a higher recurrence risk.

Stage:

Stage 0 is associated with early disease and no recurrence, while Stage 4 represents advanced disease with a higher recurrence risk. The stage combines T, N, and M variables, helping assess the overall prognosis.

Response to Treatment:

Response 1 (good response) is linked to lower recurrence risk, while Response 3 (poor response) suggests a higher likelihood of recurrence.

Recurred (Outcome):

Out of 383 patients, 108 experienced recurrence, while 275 did not.


<img width="798" alt="image" src="https://github.com/user-attachments/assets/55b7de78-5d60-49ff-aef6-fbff7a387e82" />





