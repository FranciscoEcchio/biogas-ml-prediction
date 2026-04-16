# Biogas Production Prediction using Machine Learning (Random Forest)

> This project demonstrates the application of machine learning to improve prediction and understanding of complex environmental systems such as anaerobic digestion.

---

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

After hyperparameter tuning, the models achieved:

### Biogas production
- R² ≈ 0.75  
- RMSE ≈ 97.44  
- MAE ≈ 61.03  

### VS removal
- R² ≈ 0.60  
- RMSE ≈ 11.00  
- MAE ≈ 6.88  

### Methane content
- R² ≈ 0.68  
- RMSE ≈ 5.02  
- MAE ≈ 2.91  

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

## Visualization

The following analyses were performed:

- Predicted vs actual biogas production  
- Feature importance from Random Forest  
- SHAP summary plots  

These visualizations help understand model performance and key influencing variables.

---

## Skills Demonstrated

- Machine Learning (Random Forest)  
- Data preprocessing and cleaning  
- Feature selection and engineering  
- Model training and evaluation  
- Hyperparameter tuning (GridSearchCV)  
- Environmental data analysis  
- Model interpretability (SHAP)  

---

## Tools and Technologies

- Python  
- pandas  
- scikit-learn  
- Random Forest  
- SHAP  
- Google Colab  

---

## How to Run

1. Open the Jupyter Notebook:
   `biogas_prediction_model.ipynb`

2. Install required libraries:
   - pandas  
   - numpy  
   - scikit-learn  
   - shap  

3. Run all cells to reproduce the results  

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
