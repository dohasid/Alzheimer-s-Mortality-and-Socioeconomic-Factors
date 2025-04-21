# Alzheimer-s-Mortality-and-Socioeconomic-Factors

## Project Overview
This project explores how **education**, **income**, and **mental health (depression)** relate to **Alzheimer’s mortality rates** across U.S. states. Using public datasets from the CDC, U.S. Census, and FRED, I conducted statistical analysis and visualized trends to uncover social patterns in Alzheimer’s outcomes.

## Files
- alz_project.Rmd – Full analysis code and insights
- Alzheimer's Mortality and Socioeconimic Factors.pdf – Rendered output for easy viewing

## Research Questions
- Do higher levels of education correlate with lower Alzheimer’s mortality?
- Is there a relationship between income and Alzheimer’s mortality rates?
- How does the prevalence of depression relate to Alzheimer’s mortality?

## Datasets Used
- `alzheimers.csv`: Age-adjusted Alzheimer's mortality rates by state (CDC)
- `Median Household Income data - Sheet1.csv`: State-level median income (FRED)
- `Bachelor's Attainment by Percentage - Sheet1.csv`: Education attainment rates (Census)
- `Indicators_of_Anxiety_or_Depression_Based_on_Reported_Frequency_of_Symptoms.csv`: Mental health indicators (CDC Pulse Survey)

## Methods
- Language: **R**
- Libraries: `tidyverse`, `dplyr`, `ggplot2`, `usdata`, `scales`
- Techniques:
  - Data cleaning & wrangling across multiple sources
  - State name normalization (`abbr2state`)
  - Linear regression modeling (`lm`)
  - Pearson correlation tests
  - Visualization with scatterplots, regression lines, and boxplots

## Key Findings

### Education & Alzheimer’s Mortality
- **Negative correlation** (r = -0.472, p < 0.001)
- Regression coefficient: -0.67
- Higher education = lower mortality
- Strong visual trend supported by statistical evidence

### Income & Alzheimer’s Mortality
- **Negative correlation** (r = -0.434, p = 0.0047)
- For every \$1 increase in income, Alzheimer’s mortality decreased by 0.00023
- Boxplots showed lower-income states had higher and more variable mortality rates

### Depression & Alzheimer’s Mortality
- **Positive but moderate** correlation (r = 0.36, p = 0.00998)
- Regression coefficient: 1.26
- Indicates a potential relationship, but further investigation is needed

##  Policy Recommendations
1. **Invest in Community-Based Alzheimer’s Education Programs**  
   Especially in low-income and low-education communities to promote awareness, early detection, and mental stimulation

2. **Increase Federal Funding for Alzheimer’s Research**  
   Address disparities in healthcare access and understand socioeconomic risk factors more deeply

## Visuals
- `education_vs_mortality.png`: Scatterplot with regression line
- `income_boxplot.png`: Distribution of mortality by income quartile
- `depression_vs_mortality.png`: Alzheimer’s rate vs depression rate

