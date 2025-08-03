# California-Housing-Price-Prediction
Dataset: California Housing (20,640 samples, 8 features) Target: Median House Value (in hundreds of thousands) Goal: Predict house prices using various regression techniques

📈 Key Findings
🏆 Best Performing Model

Winner: Polynomial Regression (degree=2)
Performance: R² = 0.6457, RMSE = 0.6814
Improvement over baseline: +12.1% better than Linear Regression

📊 Model Performance Ranking

Polynomial (degree=2) - R² = 0.6457 ⭐ Best
Lasso Regression - R² = 0.5769
Linear Regression - R² = 0.5758 (Baseline)
Ridge Regression - R² = 0.5758
RFE (5 features) - R² = 0.5675
Huber Regressor - R² = 0.5610
RANSAC - R² = 0.3987
Theil-Sen - R² = 0.2292

🔍 Technical Analysis
Multicollinearity Detection

High VIF features: Latitude (9.30), Longitude (8.96), AveRooms (8.34), AveBedrms (6.99)
Conclusion: Justified using Ridge/Lasso over plain OLS

Feature Importance (Linear Regression coefficients)

Latitude (-0.897) - Northern areas = lower prices
Longitude (-0.870) - Eastern areas = lower prices
MedInc (+0.854) - Higher income = higher prices
AveBedrms (+0.339) - More bedrooms = higher prices

Geographic Insights

Southern & Western California are most expensive
Income is the strongest positive predictor
Location (Lat/Long) dominates pricing

✅ Proper train-test split (80-20)
✅ Feature scaling with StandardScaler
✅ VIF analysis for multicollinearity
✅ Multiple regression techniques comparison
✅ Residual analysis and assumption checking
✅ Feature importance interpretation

Advanced Techniques

✅ Polynomial feature expansion (8 → 44 features)
✅ Regularization (Ridge/Lasso with cross-validation)
✅ Recursive Feature Elimination (RFE)
✅ Robust regression methods (Huber, RANSAC, Theil-Sen)

🎯 Key Insights
Why Polynomial Won

Captured non-linear relationships between features
70% improvement in feature count (8 → 44)
Better handling of interaction effects

Lasso Results

All 8 features retained (α = 0.001)
Indicates dataset is well-curated with minimal redundancy
Light regularization was optimal

#Results Quality

R² = 0.6457 explains ~65% of price variance
RMSE = 0.6814 represents reasonable prediction error
Strong feature importance aligns with real-world expectations

🚀 Analysis

Data preprocessing and scaling expertise
Understanding of regression assumptions
Knowledge of regularization techniques
Ability to interpret and compare models
Professional data science workflow

🎉 Conclusion
California Housing analysis was comprehensive, technically sound, and professionally executed. The polynomial regression result (R² = 0.6457) represents predictive performance for this classic dataset. Successfully identified multicollinearity, applied appropriate techniques, and provided actionable insights about the California housing market.
