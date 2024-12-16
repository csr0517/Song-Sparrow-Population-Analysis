# Song-Sparrow-Population-Analysis

## Overview
This repository contains a comprehensive data analysis report examining factors influencing song sparrow reproduction and population dynamics. The analysis investigates how female population density, nest location, and temporal factors affect breeding success in song sparrows across a 19-year study period.

## Dataset Description
- **Sample Size**: 742 observations of 356 unique birds
- **Time Period**: Data collected over 19 years (15 years of active collection)
- **Spatial Coverage**: Nest locations recorded using x-y coordinates
  - X-coordinates range: 0.25-32.83
  - Y-coordinates range: 1.375-5.250
- **Key Variables**:
  - Female population size (4-72 birds)
  - Age structure (1-7 years)
  - Reproductive output (0-12 offspring)
  - Spatial coordinates
  - Individual bird IDs

## Key Findings
1. Strong evidence for density-dependent reproduction with fewer offspring produced at higher population densities
2. Significant east-west gradient in breeding success
3. No significant north-south pattern in reproduction
4. Substantial year-to-year variation suggesting important environmental influences
5. Individual bird effects relatively modest compared to temporal effects

## Statistical Methods
- Hierarchical mixed-effects models
- Generalized Linear Mixed Models (GLMMs)
- Spatial analysis
- Model comparison using AIC
- Extensive diagnostic testing

## Technical Details
- Analyses performed in R
- Key packages used:
  - lme4
  - glmmTMB
  - DHARMa
  - mgcv
  - ggplot2

## Model Performance
- Best model: Negative Binomial GLMM
- Fixed effects explain ~10% of variance
- Full model (including random effects) explains ~36% of variance
- Significant zero-inflation detected
- No significant spatial autocorrelation in residuals

## Limitations
1. Zero-inflation in reproduction patterns
2. Some non-uniform residuals
3. Potential fine-scale spatial structures not captured
4. Missing age data for some observations

## Files
- R code: data analysis.Rmd
- Data: female.txt
- Report: Data Analysis Report.pdf
