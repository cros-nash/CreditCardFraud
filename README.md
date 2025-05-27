
# Credit Card Fraud Detection using XGBoost
---

## 📌 Project Description

This project presents an end-to-end pipeline for detecting fraudulent credit card transactions using machine learning. It combines extensive feature engineering, data visualization, model selection, and optimization techniques to build an effective fraud detection system. The final model—an XGBoost classifier—achieved an F1 score of **0.90** on Kaggle, showcasing strong performance on an imbalanced dataset.

Key highlights include:
- Custom temporal, behavioral, and category-based features.
- Exploratory data analysis to uncover correlations.
- Use of SHAP values and feature importances for explainability.
- Model tuning using performance curves and recursive feature elimination.

---

## ⚙️ Installation

### Prerequisites

Ensure you have the following installed:

- Python 3.8+
- pip
- Jupyter Notebook or JupyterLab

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/cros-nash/CreditCardFraud.git
   cd CreditCardFraud
   ```

2. Create and activate a virtual environment:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 Usage

1. Launch the Jupyter Notebook environment:
   ```bash
   jupyter notebook
   ```

2. Open and run `CreditCardFraud.ipynb`. The notebook is structured as follows:
   - Load and clean data
   - Perform exploratory data analysis
   - Generate custom features (e.g., transaction time, spending ratios, odds ratios)
   - Train initial DecisionTree model
   - Switch to and optimize XGBoost model
   - Use SHAP values and `feature_importances_` to guide final feature selection
   - Evaluate performance using F1 score, PR curve, and optimal thresholding

---

## 🌟 Features

- 📊 **EDA Visualizations**: Fraud distribution by gender, age, time of day, and geography.
- ⚙️ **Custom Feature Engineering**: Temporal indicators, spending profiles, category volatility.
- 🧠 **Model Selection**: Transition from DecisionTree to XGBoost for robustness.
- 🔍 **Interpretability**: SHAP analysis and odds ratio calculations.
- 🔄 **Recursive Feature Elimination**: Remove redundant features to avoid overfitting.
- 📈 **Threshold Tuning**: Optimize decision boundary using F1/precision-recall trade-offs.

---


## 📚 Documentation

- [ProjectPaper.pdf](./ProjectPaper.pdf): Describes the research, methodology, and technical decisions in detail.
- [CreditCardFraud.ipynb](./CreditCardFraud.ipynb): Fully executable notebook with data, models, and results.

---

## 📝 Changelog

### v1.0 (May 2025)
- Initial release
- Complete pipeline implemented
- Achieved 0.90 F1 score on Kaggle

---

## 🏁 Conclusion

A well-crafted fraud detection pipeline demonstrates both technical rigor and responsible feature design. This project highlights the importance of thoughtful preprocessing, explainable AI techniques, and real-world applicability. We hope this serves as a strong foundation for others looking to build high-performance fraud detection models.
