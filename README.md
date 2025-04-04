# basketball-performance-analysis
Basketball Player Performance Prediction (Regression Model)

# Predicting NBA Player Scoring Performance Using Regression

This project uses historical NBA statistics to build regression models that predict points scored by players based on key in-game metrics. We analyzed players by position (PG, SG, SF, PF, C), performed variable transformations, selected features, and tested multiple interaction and second-order terms to improve predictive performance.

📄 **Dataset Source:** NBA_Player_Stats.csv (Kaggle)  
📁 **Project Type:** Group project (DSC423)

---

## Project Overview

Basketball is a global sport where team strategies can benefit greatly from data-driven insights. This project analyzes 14,000+ player-season records to identify what factors most affect a player’s scoring output, based on their court position. Using regression models per position, we explored variables like effective field goal percentage, assists, rebounds, and three-point performance. Our analysis helps coaches and analysts identify the key drivers of scoring efficiency.

---

## Tools & Technologies

- R (car, caret, ggplot2)
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

- **Effective field goal %** consistently had the highest predictive power across most positions
- **Point Guards** benefited from high assists and defensive rebounding in scoring prediction
- **Shooting Guards** had nonlinear relationships with minutes played and scoring
- **Small Forwards** showed strong dependence on free throw accuracy and 3-point shooting
- **Power Forwards** scored more through free throw attempts and rebounds
- **Centers** had highest adjusted R² (0.997), scoring influenced by assists and shooting accuracy
- Final models achieved **adjusted R² values between 0.921 and 0.998**, with low RMSE

---

## Future Work

- Incorporate advanced regularization techniques (e.g., Ridge, Lasso)
- Introduce player-level time series data to track trends across seasons
- Add advanced stats (PER, usage rate, offensive rating) for richer models
- Explore clustering to group players with similar scoring profiles

---

## Files

- `notebooks/`: Contains my portion of the analysis including regression modeling, residual analysis, and cross-validation
- `images/`: Visualizations used in this README (e.g., correlation heatmaps, residual plots)
- `Project_Report.pdf`: Final group report providing full model details and cross-position comparison

---

## Contribution

This was a group project completed in DSC423. The contents included in this repo reflect **my personal contributions**, which include:

- Regression modeling for the **Point Guard** and **Small Forward** positions
- Variable transformation, multicollinearity resolution, and VIF analysis
- Residual analysis and RMSE-based model evaluation
- Co-wrote report sections related to feature selection and statistical significance

---
