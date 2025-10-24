# Longitudinal Analysis of Hemodialysis Access Types on Kidney Function

## Project Overview
Advanced statistical analysis of end-stage renal disease (ESRD) patient data to evaluate the impact of different vascular access types on kidney function recovery. This graduate-level project demonstrates sophisticated longitudinal data analysis using mixed effects models and piecewise regression.

### Research Question
How do different vascular access types (standard fistula, graft, venous transposition fistula) affect kidney function recovery (eGFR) in hemodialysis patients, and do these effects vary by patient race?

## Key Findings
- **Venous transposition fistulas** showed superior long-term eGFR improvement compared to traditional grafts
- **Standard fistulas** were associated with lower eGFR values at early time points
- **No significant racial disparities** were found in treatment effectiveness across access types
- **Piecewise regression** identified a significant change in eGFR trajectory at 20 days post-placement

## Statistical Methods

### Primary Analyses
1. **Cross-sectional Analysis**: Multiple linear regression modeling eGFR at 7 days post-placement
2. **Longitudinal Analysis**: Linear mixed effects models with:
   - Random intercepts and slopes
   - Piecewise regression (knot at 20 days)
   - Time-varying fixed effects
3. **Interaction Analysis**: Access type × race interactions

### Model Selection & Validation
- **Information Criteria**: AIC/BIC for model comparison
- **Likelihood Ratio Tests**: Random effects specification
- **Comprehensive Diagnostics**: Residual analysis, normality checks, influence diagnostics

## Quick Start

### Prerequisites
```r
install.packages(c("tidyverse", "nlme", "lme4", "ggplot2", "car"))
```
### Run Complete Analysis
- Open `statistical_analysis.RMD` in RStudio
- Install required packages if missing
- Knit the document to generate complete analysis report

## Data Description
- **Sample:** 1,255 ESRD patients from multiple US clinics
- **Design:** Observational study with repeated measures
- **Timepoints:** eGFR at 7, 20, 90, and 150 days post-access placement
- **Key Variables:** Access type, age, race, diabetes status, smoking status, BMI

## Skills Demonstrated
- **Longitudinal Data Analysis:** Mixed effects modeling, repeated measures
- **Statistical Programming:** R, tidyverse, nlme package
- **Data Visualization:** ggplot2 for clinical data trends
- **Research Methods:** Model specification, diagnostic checking, interaction analysis
- **Clinical Interpretation:** Translating statistical results to medical insights