# basketball-performance-analysis
Basketball Player Performance Prediction (DSC 423)

# Predicting NBA Player Scoring Performance Using Regression

This project uses historical NBA statistics to build regression models that predict points scored by players based on key in-game metrics. We analyzed players by position (PG, SG, SF, PF, C), performed variable transformations, selected features, and tested multiple interaction and second-order terms to improve predictive performance.

**Dataset Link:** [NBA Player Stats](https://www.kaggle.com/datasets/sadeghjalalian/nba-player-stats-19982022)

---

## Project Overview

Basketball is a global sport where team strategies can benefit greatly from data-driven insights. This project analyzes 14,000+ player-season records to identify what factors most affect a player’s scoring output, based on their court position. Using regression models per position, we explored variables like effective field goal percentage, assists, rebounds, and three-point performance. Our analysis helps coaches and analysts identify the key drivers of scoring efficiency.

---

## Tools & Technologies

- R Studio
- Regression modeling & diagnostics
- Feature selection (stepwise)
- Interaction & second-order term analysis
- VIF & multicollinearity detection
- Cross-validation (train-test split, RMSE)

---

## Methodology

- Cleaned and transformed raw dataset (14,575 rows × 31 variables)
- Split data by position: PG, SG, SF, PF, C
- Performed feature selection via backward & forward stepwise regression
- Detected and resolved multicollinearity via VIF thresholding
- Applied transformations (log, square, cube) to normalize skewed variables
- Added interaction terms and squared terms for non-linear relationships
- Performed residual analysis to validate model assumptions
- Evaluated model performance via RMSE, adjusted R², correlation coefficient

---

## Key Findings

- **Effective Field Goal %** was the strongest predictor across most positions
- **Point Guards** showed positive scoring impact from assists and defensive rebounds, with assist coefficients highly significant (p < 0.01)
- **Shooting Guards** displayed nonlinear relationships with minutes played and scoring
- **Centers** achieved the best overall model performance, with an **adjusted R² of 0.997** and low RMSE

---

## Future Work

- Use more comprehensive basketball metrics such as PER, offensive rating, and usage rate to improve prediction accuracy
- Track player performance over time to incorporate a temporal component into the model
- Explore alternative performance outcomes beyond points scored, such as efficiency rating or win shares

---

## Files

- `notebooks/`: Includes my contribution to the analysis, specifically the regression modeling, variable transformation, residual analysis, and cross-validation for the Point Guard (PG) position
- `Project_Report.pdf`: Final group report providing full model details and cross-position comparison

---
