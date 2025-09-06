# Alex Lee — Credit Card Fraud Detection (Scikit‑learn + Jupyter)

End‑to‑end notebook for detecting fraudulent credit card transactions using classical ML. Includes preprocessing, model training, class‑imbalance handling, and side‑by‑side evaluation with precision/recall/F1.

- Repository: https://github.com/1128alex/credit_card_fraud_detection

## ✨ Features
- Single Jupyter notebook pipeline: load, clean, split, train, evaluate
- Robust scaling for amount‑like features (RobustScaler)
- Multiple classifiers compared side‑by‑side:
  - Logistic Regression, Linear SVC (class_weight='balanced')
  - Random Forest, Gradient Boosting
  - Shallow Neural Network (baseline)
- Classification reports per model (precision/recall/F1, support)
- Handling extreme data imbalance
- Exported model summary to `model_report.txt`

## 🛠️ Tech Stack
- Python
- Jupyter Notebook
- pandas
- numpy
- scikit‑learn
- matplotlib (for plots)

## 📁 Project Structure
```
creditcard.csv
model_training.ipynb
model_report.txt
```

## 📊 Results (from `model_report.txt`)
```
                        Precision   Recall    f1-score
Logistic Regression
        Not Fraud       0.92        1.00      0.96
        Fraud           1.00        0.91      0.96
Shallow NN
        Not Fraud       0.92        1.00      0.96
        Fraud           1.00        0.91      0.96
Random Forest Classifier
        Not Fraud       0.89        1.00      0.94
        Fraud           1.00        0.87      0.93
Gradient Boosting Classifier
        Not Fraud       0.93        0.94      0.94
        Fraud           0.94        0.93      0.94
Linear SVC
        Not Fraud       0.93        0.99      0.96
        Fraud           0.98        0.93      0.96
```


## 🚀 Getting Started (Local)

1) Requirements
- Python

2) Set up an environment and install packages
```powershell
# From the repo root
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -U pip
pip install -r requirements.txt
```

3) Run the notebook
```powershell
jupyter notebook
```
- Open `model_training.ipynb` and run cells top‑to‑bottom.

Tips
- `creditcard.csv` is large; keep it in the project root alongside the notebook.
- If you use VS Code, you can run the notebook directly in the built‑in editor.

## 🌐 Dataset
- Standard credit card transactions dataset (local CSV: `creditcard.csv`).

## 📄 License
Please credit the author when you use parts of this repository.
