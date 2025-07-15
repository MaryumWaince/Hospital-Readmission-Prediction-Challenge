🧠 Objective
The task is to create a predictive model that can classify whether a patient will be readmitted within 30 days using historical hospital stay data.

Target Variable: Readmitted_30

1 → Patient was readmitted within 30 days
0 → Patient was not readmitted within 30 days
📁 Dataset Overview
The dataset contains structured information about hospital stays, including diagnoses, procedures, admission details, and discharge codes.

🔹 Provided Files
File Name	Description
train.csv	Training data with input features and the target variable Readmitted_30
test.csv	Testing data without the target variable
sample_submission.csv	A sample format for submitting predictions
metaData.csv	Metadata providing column definitions and value descriptions
🗂️ Features
Each row in the dataset corresponds to one hospital stay. The features include:

📅 Administrative Fields
ID – Unique stay identifier
STAY_FROM_DT – Admission date
STAY_THRU_DT – Discharge date
STAY_DRG_CD – Diagnosis-Related Group code
TYPE_ADM – Type of admission (e.g., emergency)
SRC_ADMS – Source of admission
STUS_CD – Discharge status
AD_DGNS – Primary admitting diagnosis (ICD code)
🏥 Diagnosis & Procedure Codes
The dataset includes up to 25 diagnosis codes (DGNSCD01–25) and 25 procedure codes (PRCDRCD01–25) per hospital stay.

These are based on ICD codes (International Classification of Diseases) and provide clinical insight into the patient's medical condition and treatment during the stay.

📘 Example Row
| ID | STAY_FROM_DT | STAY_THRU_DT | TYPE_ADM | SRC_ADMS | DGNSCD01 | PRCDRCD01 | ... | Readmitted_30 | |--------|--------------------|--------------------|----------|-----------|----------|------------|-----|----------------| | 122086 | 2019-01-10 00:00:00 | 2019-01-11 00:00:00 | 6 | I442 | 0JH606Z | ... | 0 |

🔍 Feature Definitions
Refer to metaData.csv for full explanations of each column, including:

Value categories for codes (e.g., admission types, discharge status)
ICD code mappings (for diagnosis and procedures)
