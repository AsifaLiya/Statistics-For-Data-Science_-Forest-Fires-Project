# Statistics-For-Data-Science_-Forest-Fires-Project
This is my project of Statistics For Data Science course on Forest Fires.
# MACHINE LEARNING MODEL- REGRESSIONS
PRESENTED BY:
- BENAZIR MEEM
- ASIFA AKTER LIYA

# INTRODUCTION:
Forest fires cause major environmental and economic damage.

<b>GOAL:</b>
Analyze factors affecting fire occurrence and size.

<b>Datasets:</b>
- Portugal Forest Fire Dataset
- Algerian Forest Fire Dataset

# DATASET DESCRIPTION (PORTUGAL):

• 517 rows, 13 columns

• Features: temp, RH, wind, rain, FFMC, DMC, DC, ISI, area

• Target: Burned area (regression)

• Data Types: Numerical + categorical (converted)

• Key Insight: Most days have zero fire area

# Dataset Description (Algeria):

• 244 rows, 14 columns (merged from 2 regions)

• Features: Temperature, RH, Ws, Rain, FFMC, DMC, DC, ISI, BUI, FWI

•Target: Classes (Fire = 1, Not Fire = 0)

• Key Insight: Dataset imbalanced with mostly 'no fire' cases.

# DATA PREPROCESSING:

• Merged datasets (Bejaia + Sidi Bel-Abbes)

• Removed null/duplicate rows

• Cleaned column names

• Converted categorical (Classes → 0/1)

• Converted features to numeric for modeling

# EDA (PORTUGAL):

- FFMC & ISI positively correlated with area

- Rain & RH negatively correlated 

- Most burned areas are small & few extreme cases

<img width="906" height="675" alt="image" src="https://github.com/user-attachments/assets/c0be725d-3232-4d6c-87db-94f00f155a62" />


# EDA (ALGERIA):

- Year and Classes columns are excluded from the correlation heatmap since they are not continuous numerical features.

- Temperature ↑ → higher fire risk (FWI)

- RH, Rain ↓ → lower fire risk

- Fire indices (FFMC, DMC, DC, ISI, BUI, FWI) highly correlated

<img width="640" height="676" alt="image" src="https://github.com/user-attachments/assets/bd2b5aca-bfaf-42c3-9f0d-6124af8b195d" />

# Plots, histogram & pie charts:
<img width="329" height="314" alt="image" src="https://github.com/user-attachments/assets/951de779-831a-43da-a70f-e4947f27c83c" /><img width="411" height="325" alt="image" src="https://github.com/user-attachments/assets/1b374db8-4d74-4f0f-aa25-01f1ebc092d6" />

<img width="483" height="345" alt="image" src="https://github.com/user-attachments/assets/1debe6a1-3563-465f-ba2f-b7f715fe0415" /><img width="493" height="339" alt="image" src="https://github.com/user-attachments/assets/55cff7b7-71ec-418d-b270-bbb8660264d6" />

# Machine Learning MODELS (PORTUGAL):
- <b>Linear Regression:</b>  Predict burned area , R2 = 0.005 (poor)

- <b>Logistic Regression:</b> Predict fire occurrence , Accuracy = 57%

# Machine Learning MODELS (ALGERIA):
- <b>Linear Regression:</b>  Predict FWI, R2 = 0.99 (excellent)
- <b>Logistic Regression:</b>  Predict fire occurrence, Accuracy = 98%
- <b>Decision Tree Classifier:</b>  Predict fire occurrence, Accuracy = 98%, same as logistic regression

# KEY FINDINGS:
- Humidity & Rain → Less fire risk
- Portugal dataset: predicting fire size difficult
- Algerian dataset: highly predictive for fire occurrence
- Temperature, FFMC, ISI, FWI → More fire risk

# CONCLUSION:

- Forest fires are predictable using environmental & fire indices.

- Portugal dataset → difficult due to skewed fire size values.

- Algerian dataset → ML models achieved 98% accuracy.

- Models can support fire risk prevention & forest management.
