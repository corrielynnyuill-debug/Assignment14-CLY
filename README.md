# Assignment14-CLY
Assignment 14 Ethical AI Analysis and Explainability

Income Classification with Fairness & Explainability
This project analyzes the UCI Adult Income dataset to predict whether an individual earns more than $50K per year. Beyond standard machine learning modeling, the project focuses on ethical AI, including fairness evaluation and model explainability using SHAP and LIME.
Project Objectives
•	Build a predictive model for income classification
•	Evaluate fairness across demographic groups (sex)
•	Apply SHAP and LIME to interpret model behavior
•	Discuss ethical considerations and potential mitigation strategies
Dataset
The dataset includes demographic and employment-related attributes such as:
•	Age
•	Education level
•	Hours worked per week
•	Occupation
•	Capital gain/loss
•	Sex, race, marital status
Target variable:
•	>50K
•	<=50K
Methods
Preprocessing
•	One hot encoding for categorical features
•	Standard scaling for numerical features
•	Train/test split
•	Pipeline for reproducibility
Model
•	Logistic Regression
•	Threshold calibration to address class imbalance
•	Binary label encoding for fairness metrics
Fairness Analysis
Fairness was evaluated using Fairlearn across the sensitive attribute sex.
Key metrics:
•	Selection Rate
•	True Positive Rate (TPR)
•	False Positive Rate (FPR)
•	Accuracy
Findings:
•	Males received higher selection rates and TPR
•	Females experienced slightly higher FPR
•	Indicates moderate fairness disparities
Explainability
SHAP
•	Identified global feature importance
•	Key drivers: capital-gain, education-num, age, hours-per-week
•	Waterfall plots provided local explanations for individual predictions
LIME
•	Confirmed SHAP insights with interpretable local explanations
•	Highlighted how specific features influenced a single prediction
Ethical Considerations
•	Dataset reflects historical socioeconomic biases
•	Model shows measurable disparities across sex
•	Recommendations include: 
o	Rebalancing data
o	Trying alternative models
o	Applying fairness mitigation algorithms
o	Intersectional fairness analysis
Summary
This project demonstrates how to combine predictive modeling with fairness evaluation and explainability techniques to build more transparent and responsible AI systems.
