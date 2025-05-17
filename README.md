# Bank Loan Classification

## Overview

This is an older project from my early journey in data science, focused on understanding what factors influence whether a person gets approved for a bank loan. Although basic compared to more advanced projects I've done, it remains an excellent demonstration of end-to-end classification modeling, handling imbalanced datasets, and interpreting feature importance.

## Methods Used

- **Models**: Logistic Regression, Decision Tree, Random Forest  
- **Data Preprocessing**:
  - Standardization of numerical variables
  - Label encoding for categorical fields
- **Imbalanced Data Handling**:  
  - Applied **SMOTE (Synthetic Minority Oversampling Technique)** to address significant class imbalance (few approved loans vs many denied).
  - SMOTE helped the models generalize better by generating synthetic examples of the minority class.
- **Train/Test Split**: 80/20

## Results

Random Forest performed best in terms of accuracy, precision, and recall.

**Accuracy:** 0.98  
**Precision:** 0.90
**Recall:** 0.92

### Model Performance Visualization

![Model Results](./results/performance.png)  

## Key Variables and Why They Matter

1. **Income**  
   Higher income generally suggests better repayment capacity, making it a natural indicator for loan eligibility.

2. **Education Level**  
   Those with higher education levels often have more stable or higher-paying jobs, which can influence a bank’s decision.

3. **Family Size**  
   A larger family might imply a greater financial burden, possibly affecting repayment ability. Smaller families may be seen as lower risk.

4. **Average Credit Card Usage**  
   High usage might signal either good credit activity or potential overextension. Used in moderation, it can reflect responsible credit behavior.
