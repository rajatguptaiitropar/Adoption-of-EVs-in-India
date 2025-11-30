Project README: 

**Modelling and Analysis of Electric Vehicle Adoption in India**

 **Overview**
This project focuses on understanding and predicting consumer choice between Electric Vehicles (EVs) and Conventional Vehicles (CVs) in India, using Chandigarh as a case study for localized policy insight. The primary goal was to create an accurate predictive model that quantifies the precise non-linear utility consumers derive from various vehicle attributes.

 **Objectives**
The project fulfilled the following key objectives:

Key Factor Identification: Determined the most salient factors influencing EV adoption, including price difference, driving range, and financial incentives.

Data Collection & Survey Design: Executed a robust Stated Preference (SP) survey across targeted consumer income segments in Chandigarh, resulting in approximately 3,220 individual choice

Model Implementation: Implemented a non-linear Multi-Layer Perceptron (MLP) Artificial Neural Network (ANN) model to predict the probability of EV choice, justified by its superiority over traditional linear models.

Policy Formulation: Translated technical findings from the model into prioritized, actionable, and segment-specific policy recommendations for government bodies and manufacturers.

 **Methodology**
Data Acquisition
Method: Stated Preference (SP) Survey.
Location: Five main public places in Chandigarh (e.g., Sector 17, Elante Mall,sector 22, sector 28,sukhna lake).
Dataset Size: Over 300 valid responses, yielding approximately 3,220 total choice observations.
Key Attributes: Purchase price, operating cost, driving range, subsidy amount, registration discount, and charging availability.

**Modelling**

Model Type: Multi-Layer Perceptron (MLP) Artificial Neural Network (ANN).

Architecture: Feedforward topology with two hidden layers (ReLU activation) and a Sigmoid output layer to predict P(Choice=EV).
Training Protocol: Trained using Binary Cross-Entropy loss and the Adam optimizer over 100 epochs.

 **Key Findings & Policy Implications**
Finding Category	Key Analytical Result	Policy Recommendation
Dominant Disutility	
Price Difference (EV Price – CV Price) is the largest negative factor influencing consumer choice across all segments.
Government should prioritize Point-of-Sale Subsidies (e.g., FAME-III schemes) to directly reduce the capital cost hurdle.
Dominant Utility	
Driving Range provides the largest positive utility, with non-linear increases in preference once critical thresholds are surpassed.
Regulatory bodies should enforce a minimum mandatory range standard of 180 km for all new EVs, as this significantly mitigates range anxiety.
Infrastructure Impact	
Charging Time is identified as a significant disutility factor.
Invest in and standardize Fast Charging infrastructure (DC charging) to reduce the functional disutility of time cost and alleviate range anxiety.
Model Performance	
Model achieved a peak Validation Accuracy of 88.42% and ROC AUC scores consistently exceeded 0.95 across all consumer segments, confirming high predictive power.

Model Explainability: Advanced interpretability analyses, including SHAP (SHapley Additive ExPlanations), were used to quantify the exact contribution of each attribute to the prediction.

Classification Bias: Error analysis revealed a consistent conservative classification bias (approx. 2:1 False Negative to False Positive ratio), meaning the model is more likely to under-predict EV adoption than over-predict it. This suggests that forecasts based on the model represent a reliable, cautious estimate of minimum market demand.


Expanding the data collection geographically across other Indian cities to validate the generalizability of the model architecture.

Integrating public infrastructure data (current charging point locations) as a feature to refine the spatial recommendations.
