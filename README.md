# AI-and-EQUITY-in-HEALTHCARE
Overview
This project analyzes hospital readmission prediction models using the Diabetes 130-Hospitals dataset, focusing on fairness, bias detection, and model performance. The goal is to develop machine learning models that not only predict 30-day readmission rates accurately but also ensure fair treatment across gender groups.

Key Features
ML Model Development: Trained and evaluated models to predict patient readmission.
Fairness Analysis: Assessed bias in predictions, particularly false negative rate (FNR) parity across gender groups.
Bias Mitigation Techniques: 

Implemented:

Hyperparameter Tuning: Improved accuracy and precision
Exponentiated Gradient (EG): Reduced bias while maintaining performance.
Threshold Optimizer (TO): Minimized FNR while maximizing recall.

Performance Trade-Offs: Compared models based on accuracy, recall, FNR, and fairness metrics.

Results & Insights
Hyperparameter tuning improved accuracy but increased bias slightly.
EG (ε = 0.01) achieved the best fairness across multiple metrics.
TO with FNR parity constraint significantly reduced FNR while increasing recall, but at the cost of higher FPR.

Key takeaway: Choosing the optimal model depends on whether the focus is overall accuracy, bias reduction, or fairness in false negatives.

Python Libraries Used : Scikit-learn, Fairlearn, Aequitas

Future Improvements
Extend fairness analysis to race, age, and other protected attributes.
Experiment with additional bias mitigation techniques.
Deploy as a fairness-aware hospital readmission prediction API.
