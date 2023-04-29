Weekly Progress Report: 4-28
Albert Wang - Kaggle Progress

Progress/Insights:
- Did more EDA, identified multiple columns with single-values, removing them as they have no predictive power.
- Used k-NN imputation to fill in the instances with missing values.
- Performed PCA on the 756 remaining features, yielding 20 components that can explain 71% of the original variance. 
- Plotting the distribution of target values showed that the targets are extremely right skewed, with most observations falling below 40, and the vast majority falling below 20. 

Problems/Challenges:
- A prominent potential challenge is the restriction of the target range, being [0,100]. A standard regression does not have a restricted range of possible values it may predict.

Plan/Next Steps:
- Emailed Prof Shi to ask for advice on the restricted range problem. 
- Attempt various regression models with the dim-reduced features and check score.
- Models to try: LinearRegression, RandomForestRegressor, MARS?