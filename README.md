# Social Interaction in International Schools

**Author:** Coté Osimani  
**Date:** November 17, 2022  

## Overview
This project analyzes survey data on **social interactions** among students in international school settings, with a focus on differences between **control** and **treatment** groups.  
The analysis evaluates:
- Willingness to interact with peers from different nationalities.
- The role of nationality, language proficiency, and prior international experience.
- Regional differences in interaction patterns.
- Potential effects of treatment on social integration.

## Data
- **Survey file:** `survey.csv` (local path in script).  
- **Key variables:**  
  - Demographics (age, gender, nationality, socioeconomic status).  
  - Language skills and number of languages spoken.  
  - Study and work experience abroad.  
  - Interaction patterns (with Germans, with other internationals, with co-nationals).  
  - 10 outcome variables measuring willingness to interact.

## Methods
1. **Data Cleaning:**
   - Filtered by consent.
   - Removed incomplete responses.
   - Converted categorical responses to numeric/dummy variables.
   - Created aggregate measures like `willingness` score.
2. **Descriptive Statistics:**
   - Regional distributions.
   - Group means by nationality and treatment status.
3. **Statistical Analysis:**
   - Correlation matrix of outcomes.
   - Density and box plots comparing groups.
   - Control-treatment balance checks (t-tests, Wilcoxon tests).
4. **Regression Models:**
   - OLS models predicting willingness with varying controls (abroad experience, interaction patterns, living situation, region dummies).

## R Packages
`tidyverse`, `countrycode`, `stargazer`, `stringr`, `ggplot2`

## Output
- Summary tables and descriptive stats.
- Visualizations:
  - Density plot of willingness by treatment.
  - Boxplot of willingness by interaction type and treatment.
- Regression outputs (5 models with incremental controls).

## License
MIT License – see `LICENSE` file.
