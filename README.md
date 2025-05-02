# LVMI-Prediction-EAT-Impact-Analysis-using-Clinical-Data
Project Description:
This project aims to predict Left Ventricular Mass Index (LVMI) — a critical indicator of heart health — using echocardiographic and clinical features, with a special focus on evaluating the impact of Epicardial Adipose Tissue (EAT) thickness measured at two different positions: PLAX and PASX.
A regression-based machine learning approach was used to build a predictive model for LVMI and statistically evaluate the influence of each feature.
________________________________________
Key Objectives:
•	Predict LVMI using relevant cardiac and clinical features.
•	Analyze the effect of EAT thickness on LVMI.
•	Evaluate feature importance using both Random Forest and ANOVA F-test.
•	Apply OLS regression to extract feature weights, statistical significance (p-values), and confidence intervals.
•	Calculate evaluation metrics like R² Score, MSE, and AUC.
•	Determine whether a clinical threshold of EAT can be used to flag high LVMI patients.
________________________________________
Key Features Used in Modeling:
•	LVM, LVEDd, IVSd, PWd — standard echocardiographic measurements.
•	EAT from PLAX at end diastole
•	EAT from PASX at end diastole
•	E/'e ratio (diastolic function)
•	HTN (Hypertension status)
•	EF % (Ejection Fraction)
•	Age
________________________________________
Techniques and Tools:
•	Data cleaning: duplicate removal, categorical normalization, outlier handling.
•	Feature encoding: binary and one-hot encoding.
•	Feature scaling: StandardScaler.
•	Feature selection: RandomForest Classifier, SelectKBest (ANOVA F-test).
•	Regression modeling: OLS, LinearRegression.
•	Model evaluation: R² = 0.97, MSE ≈ 41.6, AUC ≈ 0.95.
•	Threshold detection: Distribution-based analysis of EAT for high-LVMI cases.
________________________________________
 Key Insights:
•	EAT values showed a measurable but not statistically significant effect on LVMI individually (p > 0.05).
•	IVSd, PWd, and LVEDd were the most influential predictors of LVMI (high positive weights and significant p-values).
•	The model demonstrated high accuracy and generalization with an R² of 0.97 on the training set.
•	A preliminary EAT threshold (around 6 mm) was identified where LVMI values tend to exceed normal levels, suggesting potential for risk stratification.
________________________________________
 Conclusion:
This model can be integrated into a clinical decision support system to assist in early detection of LVH (Left Ventricular Hypertrophy) and evaluate the role of EAT as an emerging cardiovascular risk marker. The framework is extendable to larger datasets and may benefit from longitudinal data to further validate the predictive value of EAT.
________________________________________

