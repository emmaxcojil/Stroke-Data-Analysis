This project involves the analysis and enhancement of general practice medical records to identify stroke events and analyze patient characteristics. The primary goal is to integrate patient personal information with their medical records, identify stroke occurrences, and derive insights from the data.

Dataset Description
The project utilizes three anonymized and modified text files containing general practice records:

cases_personal.txt: Contains personal information of patients, including sex and date of birth.
cases_medical.txt: Contains medical records for the patients.
stroke_codes.txt: Contains a list of medical codes corresponding to stroke events.

Variables
The datasets include the following variables:

idno: Patient identification number.
dob: Date of birth.
sex: Sex of the patient (1 = male, 2 = female).
evntdate: Date when the patient consulted with the practice.
medcode: Medical codes for symptoms, diagnoses, doctor actions (e.g., ordering a blood test), or drugs prescribed.
description: Text description of the medical codes.

Data Enhancement Steps
The following enhancements were made to the cases_medical.txt file:

Merging Personal Information: Added patients' personal information (dob and sex) to each of their medical records by merging with cases_personal.txt using idno.

Identifying Stroke Records: Generated a binary variable is_stroke for each medical record to indicate whether it corresponds to a stroke event. This was determined by checking if the medcode exists in the stroke_codes.txt list.

Calculating Age at First Stroke: For each patient, calculated the age at their first stroke occurrence and added this as a new variable age_at_first_stroke to their medical records.

Summary of Findings
Personal Information of the Study Population
Gender Distribution: Detailed the proportion of male and female patients in the study.
Age Distribution: Analyzed the age range of patients, providing insights into the demographics.
Characteristics of Stroke Patients
Incidence of Stroke: Identified the number of patients who experienced a stroke.
Age at First Stroke: Analyzed the average and distribution of ages at which patients had their first stroke.
Gender and Stroke: Explored any correlations between patient sex and stroke occurrence.

Additional Insights
Consultation Patterns: Examined the frequency of medical consultations among patients.
Common Medical Codes: Identified the most frequent medical codes and their descriptions in the dataset.
Age Correlation: Checked if there is continuous hospital visits after first stroke event
