# Biogas Production Prediction using Machine Learning (Random Forest)

## Project Overview
Anaerobic digestion is a complex biological process widely used for biogas production from organic waste. However, predicting its performance is difficult due to nonlinear interactions between multiple variables.

This project applies machine learning techniques to model and predict biogas production from brewery waste, improving understanding and potential optimization of the process.

---

## Objectives

- Identify key variables influencing anaerobic digestion performance  
- Develop predictive models for:
  - Biogas production (mL/g VS)
  - Volatile solids (VS) removal (%)
  - Methane content (CH₄ %)  
- Evaluate model performance and interpret results  

---

## Dataset

The dataset was built from experimental data on anaerobic digestion of brewery residues, including:

- Brewery spent grain  
- Residual yeast  
- Wastewater  

### Input Variables
- Total Solids (TS)  
- Volatile Solids (VS)  
- Chemical Oxygen Demand (COD)  
- Carbon/Nitrogen ratio (C/N)  
- pH  
- Temperature  
- Hydraulic Retention Time (HRT)  
- Organic Loading Rate (OLR)  
- Inoculum type and source  

### Target Variables
- Biogas production (mL/g VS)  
- VS removal (%)  
- Methane content (%)  

---

## Methodology

### Data Preprocessing
- Data cleaning and standardization  
- Handling missing values  
- Detection of outliers and unrealistic values  
- Feature selection and categorization  

### Model Development
- Train-test split (80/20)  
- Random Forest Regressor  
- Hyperparameter tuning using GridSearchCV  

### Evaluation Metrics
- R² (coefficient of determination)  
- RMSE (Root Mean Square Error)  
- MAE (Mean Absolute Error)  

---

## Results

The models showed solid predictive capability, especially after hyperparameter tuning:

- **Biogas production model**: highest predictive performance  
- **VS removal model**: moderate accuracy  
- **Methane content model**: more variable performance  

These results reflect the inherent complexity and variability of anaerobic digestion systems.

---

## Model Interpretability

To better understand model behavior:

- Feature importance analysis was performed  
- SHAP (SHapley Additive exPlanations) was applied  

### Key Insights
- Biogas production is strongly influenced by substrate composition and operational conditions  
- Some variables have nonlinear and interacting effects  
- Machine learning helps uncover relationships not captured by traditional methods  

---

## Tools and Technologies

- Python  
- pandas  
- scikit-learn  
- Random Forest  
- SHAP  
- Google Colab  

---

## Key Contributions

- Application of machine learning to an environmental engineering problem  
- Integration of experimental data from multiple studies  
- Identification of critical variables in anaerobic digestion  
- Demonstration of predictive modeling in complex biological systems  

---

## Conclusion

This project demonstrates that Random Forest models can effectively predict biogas production and capture nonlinear relationships in anaerobic digestion systems.

The approach provides a valuable tool for:

- Process optimization  
- Performance prediction  
- Decision-making in waste-to-energy applications  

---

## Future Work

- Expand dataset size and diversity  
- Test alternative machine learning models  
- Develop real-time prediction tools  
- Apply models to industrial-scale systems  
