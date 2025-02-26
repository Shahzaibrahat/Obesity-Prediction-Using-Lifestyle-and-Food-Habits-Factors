# Obesity Prediction Based on Lifestyle and Food Habits

## Overview
This project aims to predict obesity levels based on individuals' lifestyle choices and food consumption habits. The study identifies key contributors to obesity and provides insights for healthcare professionals, researchers, and individuals to promote healthier lifestyle choices.


## Repository Structure
```
📂 project_root/
│-- 📂 Code_file.Rmd             # Raw and processed dataset
│-- 📜 report_with_visulaizations.pdf        # R Markdown report containing analysis and findings
│-- 📜 README.md         # This file
```


## Dataset
The dataset contains 2,111 records of individuals from Mexico, Peru, and Colombia, aged 14 to 61. It includes 17 attributes related to:
- **Lifestyle factors**: Gender, age, smoking status, physical activity, screen time, transportation mode.
- **Food habits**: High-caloric food intake, vegetable consumption, number of meals, snacks, alcohol intake, and water consumption.
- **Target Variable**: Obesity levels categorized from Insufficient Weight to Obesity Type III based on WHO standards.

## Exploratory Data Analysis (EDA)
EDA was conducted to visualize key relationships between obesity levels and various features:
- **BMI Boxplot**: Highlights outliers in certain obesity categories.
- **Stacked Bar Plot**: Shows gender distribution across obesity levels.
- **Family History Bar Graph**: Indicates strong correlation between family history and obesity levels.
- **Bubble Chart**: Depicts weight distribution trends across obesity levels.

## Methodology
Several machine learning models were evaluated for obesity prediction:
- **Linear & Polynomial Regression**: Poor performance due to non-linearity.
- **Decision Tree**: Accuracy of 59.34%, struggled with recall in some categories.
- **Random Forest**:
  - **Food Habits Dataset**: 69.98% accuracy.
  - **Lifestyle Habits Dataset**: 61.23% accuracy.
  - **Combined Dataset (Tuned Model)**: Achieved **84.16% accuracy**, outperforming individual models.
- **Logistic Regression**: 86% accuracy but high false positives, making it less reliable.

## Conclusion
- The **Random Forest model** using both food habits and lifestyle factors provides the best prediction accuracy (84.16%).
- The model highlights the importance of dietary habits and lifestyle choices in determining obesity levels.
- The findings can aid in designing targeted health interventions and preventive measures.


## Acknowledgments
This study is based on publicly available obesity data and aims to provide valuable insights for public health research and intervention strategies.




