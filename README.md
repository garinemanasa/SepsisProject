
# Sepsis

Sepsis is a life-threatening condition that affects 1.7 million people in the U.S. annually, leading to 270,000 deaths. It contributes to over one-third of hospital fatalities and accounts for $24 billion in healthcare costs annually.

Despite its severity, early detection remains a challenge due to sepsis' syndromic nature, often leading to delayed treatment and poor patient outcomes. This project aims to develop a data-driven approach to early sepsis detection.

## Table of Contents
- [Dataset Overview](#dataset-overview)
- [Project Goals](#project-goals)
- [Demographic Analysis](#demographic-analysis)
  - [Patient Distribution](#patient-distribution)
  - [ICU Admissions](#icu-admissions)
  - [Gender Distribution](#gender-distribution)
  - [Age and Gender Analysis](#age-and-gender-analysis)
  - [ICU Length of Stay (ICULOS)](#icu-length-of-stay-iculos)
  - [Onset Sepsis](#onset-sepsis)
  - [Patient Admission Patterns](#patient-admission-patterns)
- [Lactate Analysis](#lactate-analysis)
- [Kidney Analysis](#kidney-analysis)
- [Systemic Inflammatory Response Syndrome (SIRS)](#systemic-inflammatory-response-syndrome-sirs)
- [Conclusion](#conclusion)

## Dataset Overview
- 1.5 million+ data points from 40,000+ ICU patients
- Hourly patient records, including vitals, demographics, and lab results
- Sepsis diagnosis labels indicating the hour of onset
- 34 key biomarkers related to sepsis progression

## Project Goals
- **Early Sepsis Detection**: Develop predictive models to detect sepsis risk hours before diagnosis.
- **Feature Engineering**: Extract meaningful insights from demographic, lab, and vital sign data.
- **Time-Series Analysis**: Analyze hourly trends to understand sepsis progression.
- **Clinical Decision Support**: Provide real-time risk scores to assist ICU clinicians.

## Demographic Analysis

<img width="1116" alt="sepsis Demographic analysis" src="https://github.com/user-attachments/assets/d8bbb7a4-624b-48df-82d5-1f2c565a74ff" />


### Patient Distribution
- Total patients: 40,336
- Sepsis incidence: 7.27% (2,932 patients)
- Non-sepsis patients: 98.94% (37,404 patients)

### ICU Admissions
- MICU sepsis admissions: 1.5% (189 patients)
- SICU sepsis admissions: 2.97% (87 out of 2,932 patients)
- Non-sepsis MICU admissions: 12,078 patients
- Non-sepsis SICU admissions: 12,365 patients

### Gender Distribution
- Female patients: 44.05%
- Male patients: 55.95%

### Age and Gender Analysis
- Patients classified into ten age groups
- Male patients showed higher susceptibility to sepsis across age groups

### ICU Length of Stay (ICULOS)
- Sepsis patients: Shorter ICU stays compared to non-sepsis patients
- Onset sepsis patients: Longest ICU stays
- Average ICU stay for sepsis patients (excluding onset): 55.26 hours

### Onset Sepsis
- Percentage of onset sepsis patients: 6.21%
- Distribution visualized based on ICU Length of Stay

### Patient Admission Patterns
- Relationship established between patient volume and hospital admission time
- Gender-specific variations in admission times for sepsis patients
- MICU and SICU patient counts fluctuated during the first 24 hours of admission
- Highest count in the 1st hour
- Decreasing trend towards the 24th hour

This demographic analysis provides crucial insights into patient distribution, sepsis incidence, and ICU utilization patterns. These findings can inform strategies for optimizing patient care and resource allocation.

## Lactate Analysis

Lactate Monitoring focuses on tracking lactate levels in ICU patients to assess sepsis risk and treatment response. Lactate is a key biomarker of tissue oxygenation, and its elevation is often linked to high risk.

<img width="926" alt="Lactate analysis" src="https://github.com/user-attachments/assets/fe171d7a-8c2e-47ad-ac8e-0328049f07f0" />


### Key Insights
- **Lactate Clearance Correlates with Survival**: Reducing lactate levels is linked to lower mortality.
- **Persistent Hyperlactemia Signals Poor Prognosis**: Requires urgent medical intervention.
- **Sepsis and Septic Shock Are Major Causes**: Alongside cardiac arrest, respiratory failure, and metabolic disorders.

## Kidney Analysis

<img width="950" alt="kidneyanalysis" src="https://github.com/user-attachments/assets/7a80d0f1-eb98-4d41-8d6d-65ae28719ac9" />


### Estimated Glomerular Filtration Rate (eGFR)
- Normal eGFR: ≥ 90
- Abnormal eGFR Stages:
  - Early Stage: 89–60
  - Kidney Disease: 59–15
  - Kidney Failure: < 15

### Key Findings
- 26% of patients exhibit normal eGFR.
- 31.96% have kidney disease.
- 17.05% are experiencing kidney failure.
- 16% fall into the early stages of kidney abnormalities.

### ICU Admission Analysis by Unit
- **Unit 1 (MICU)**:
  - 220 kidney failure cases
  - 316 kidney disease cases
- **Unit 2 (SICU)**: A comparatively lower admission rate.

## Systemic Inflammatory Response Syndrome (SIRS)

<img width="688" alt="Sirs" src="https://github.com/user-attachments/assets/f1197e51-8e0b-4aba-bcee-485954e163a5" />


### Key Observations
- **Heart Rate**: Patient ID 3516 had a Heart Rate of 94 bpm at Trigger Hour 10.
- **Respiratory Rate**: Patient ID 9 recorded a Respiratory Rate of 30 bpm during the Trigger Hour.
- **WBC Count and PaCO2**: Patient ID 8 had a WBC Count of 11.4 and PaCO2 of 25 mmHg during the Trigger Hour.
This study emphasizes the importance of monitoring key biomarkers such as Temperature, Heart Rate, Respiratory Rate, PaCO2, and WBC Count for timely identification and management of SIRS.

### Conclusion
The analysis provides valuable insights into sepsis detection, patient demographics, and ICU utilization patterns,Lactate Analysis,Kidney Analysis,SIRS. These findings can aid clinicians in early diagnosis and effective management of sepsis, improving patient outcomes.
