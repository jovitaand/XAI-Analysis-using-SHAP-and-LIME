# XAI-Analysis-using-SHAP-and-LIME

This project explores Explainable AI (XAI) techniques, specifically SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-agnostic Explanations), to understand and interpret predictions from a machine learning model designed to assess 30-day readmission risks for diabetes patients.

## Why Explainability in AI?
Complex AI models often function as "black boxes," with decision-making processes that are difficult to interpret. Explainability enhances:
- **Trust**: Users can understand and trust AI decisions.
- **Accountability**: Organizations can ensure ethical compliance, especially in fields like healthcare.
- **Fairness**: Transparency in decision-making helps to identify and reduce biases.

## Project Structure
- **Data**: Uses a clinical dataset tracking hospital readmissions for diabetes patients.
- **Model**: A logistic regression model predicts patient readmission risk.
- **XAI Techniques**:
  - **SHAP**: Calculates feature importance based on Shapley values for global model interpretability.
  - **LIME**: Generates local explanations for individual predictions, focusing on specific instances.

## Installation
Ensure the required libraries are installed:
```bash
pip install shap lime scikit-learn tensorflow pandas matplotlib seaborn
```
## Usage
- **Data Loading**: Load the dataset and preprocess by creating dummy variables for categorical features.
- **Model Training**: Train a logistic regression model and evaluate performance using balanced accuracy and ROC curves.
- **Explainability**:
  - **LIME**: Use `LimeTabularExplainer` to visualize explanations for individual predictions.
  - **SHAP**: Initialize `shap.initjs()` and use `LinearExplainer` for global feature importance visualization.

## Important Notes
- **Visualization Error**: If SHAP plots do not render, ensure `shap.initjs()` is called at the beginning of the notebook. For full interactivity, use Jupyter Notebook rather than JupyterLab.
- **Key Files**:
  - `Lab Notebook 5.ipynb`: Contains detailed analysis, model training, and XAI visualization steps.

## License
- This README in Markdown is ready for GitHub or any markdown-supported platform. Let me know if any other sections are needed!



