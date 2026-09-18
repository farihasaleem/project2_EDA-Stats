# project2_EDA-Stats
# Diabetes Risk Analysis

Exploratory data analysis and statistical investigation of a diabetes risk dataset 
(~15,000 patient records), examining which health and lifestyle factors most strongly 
relate to diabetes risk classification (Low / Moderate / High).

## Dataset
Patient-level data including demographics (age, gender, city), lifestyle factors 
(physical activity, diet, smoking, sleep, stress), and medical readings (fasting 
blood sugar, HbA1c, blood pressure, BMI, waist circumference).

## Key Findings
- **Fasting blood sugar (correlation: 0.74)** and **HbA1c level (0.73)** are by far 
  the strongest predictors of diabetes risk — far stronger than age, BMI, or lifestyle 
  factors.
- High-risk patients average 226.5 mg/dL fasting blood sugar vs. 148.3 mg/dL for 
  low-risk patients — a gap of nearly 80 points.
- BMI and waist circumference are nearly redundant (0.94 correlation), as are 
  fasting blood sugar and HbA1c (0.91) — both pairs largely measure overlapping 
  information, worth noting for feature selection in any future predictive model.
- Sleep and stress show a moderate negative correlation (-0.38): patients reporting 
  less sleep tend to report higher stress.

## Tools
Python, pandas, seaborn, matplotlib

## Next Steps
A follow-up project will use this dataset to train a classification model 
predicting diabetes risk from these features.
