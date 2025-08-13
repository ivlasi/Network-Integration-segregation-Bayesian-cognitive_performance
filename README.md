# Network-Integration-segregation-Bayesian-cognitive_performance
This analysis calculates both brain network integration and segregation metrics from functional connectivity data, then uses a Bayesian regression framework to examine their relationship with cognitive performance. Network metrics serve as predictors, cognitive test scores as the outcome.
# Network Integration & Segregation Analysis with Bayesian Modeling

## Overview
We investigate large-scale brain network organization and its links to cognitive function using neuroimaging-derived connectivity measures.  
The workflow includes:
1. **Network Integration & Segregation Calculation** – derived from functional connectivity matrices (e.g., Yeo 7-network parcellation).
2. **Bayesian Regression Modeling** – statistical modeling to estimate relationships between network metrics and cognitive test scores, while accounting for covariates (age, sex, education).

## Bayesian Model Description
The Bayesian regression model:
- Uses network integration and segregation as predictors.
- Includes cognitive performance scores as the dependent variable.
- Adjusts for covariates such as age, sex, and education.
- Produces posterior distributions for all parameters, enabling the calculation of credible intervals and probabilities for effect direction.

## Requirements
- Python 3.9+
- NumPy
- Pandas
- Matplotlib
- Statsmodels
- CmdStanPy (or other Bayesian modeling library)
- ArviZ

Install dependencies with:
```bash
pip install -r requirements.txt
