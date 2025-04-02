# AI-and-EQUITY-in-HEALTHCARE
**Overview**
This project analyzes hospital readmission prediction models using the Diabetes 130-Hospitals dataset, focusing on fairness, bias detection, and model performance. The goal is to develop machine learning models that not only predict 30-day readmission rates accurately but also ensure fair treatment across gender groups.

**Key Features** <br />
ML Model Development: Trained and evaluated models to predict patient readmission. <br />
Fairness Analysis: Assessed bias in predictions, particularly false negative rate (FNR) parity across gender groups. <br />
Bias Mitigation Techniques: 

**Implemented:** <br />
Hyperparameter Tuning: Improved accuracy and precision <br />
Exponentiated Gradient (EG): Reduced bias while maintaining performance. <br />
Threshold Optimizer (TO): Minimized FNR while maximizing recall.

**Performance Trade-Offs:** Compared models based on accuracy, recall, FNR, and fairness metrics.

**Results & Insights** <br />
Hyperparameter tuning improved accuracy but increased bias slightly. <br />
EG (ε = 0.01) achieved the best fairness across multiple metrics. <br />
TO with FNR parity constraint significantly reduced FNR while increasing recall, but at the cost of higher FPR.

**Key takeaway:** Choosing the optimal model depends on whether the focus is overall accuracy, bias reduction, or fairness in false negatives.

**Python Libraries Used :** Scikit-learn, Fairlearn, Aequitas

**Future Improvements**
Extend fairness analysis to race, age, and other protected attributes.<br />
Experiment with additional bias mitigation techniques.<br />
Deploy as a fairness-aware hospital readmission prediction API.<br />
