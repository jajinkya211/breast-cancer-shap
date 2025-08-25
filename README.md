This project benchmarks multiple machine learning models for breast cancer diagnosis using the Wisconsin Breast Cancer dataset, with a focus on model explainability through SHAP (SHapley Additive exPlanations).

Key Steps Implemented

Dataset Exploration & Preprocessing

Loaded the Wisconsin Breast Cancer dataset from scikit-learn.

Performed exploratory data analysis (EDA) to understand class distribution and feature importance.

Normalized and scaled features to improve training stability.

Split the dataset into training and test sets using stratified sampling to preserve class balance.

Model Development

Implemented Logistic Regression as a baseline linear classifier.

Trained and tuned XGBoost, leveraging gradient boosting for nonlinear decision boundaries.

Built a lightweight PyTorch MLP (Multi-Layer Perceptron) with early stopping to benchmark against tree-based methods.

Applied cross-validation to evaluate consistency and reduce variance in reported results.

Model Evaluation

Computed accuracy, ROC-AUC, precision, recall, and confusion matrices.

Compared learning curves across models to diagnose overfitting/underfitting.

Summarized model performance in both numerical tables and plots.

Explainability with SHAP

Used TreeExplainer for XGBoost and KernelExplainer for other models.

Generated SHAP summary plots to visualize global feature importance.

Created bar plots for top contributing features across all patients.

Produced per-instance explanations (force plots) to interpret individual predictions.

Demonstrated how SHAP values align with clinical interpretability (e.g., identifying radius, texture, and smoothness as key features).

Documentation & Reproducibility

Exported the notebook as a Colab-friendly PDF for easy sharing.

Provided environment files (requirements.txt and environment.yml) for reproducibility.

Added licensing, citation metadata, and contribution guidelines to make the project shareable and citable.

Outcomes

Showed that XGBoost consistently outperformed Logistic Regression and the small MLP in accuracy and ROC-AUC on this dataset.

Demonstrated how SHAP explanations can make black-box models more interpretable by clearly identifying feature contributions.

Produced a reproducible and well-documented workflow that can be extended to other medical datasets.
