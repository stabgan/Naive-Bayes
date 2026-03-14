# Naive Bayes Classifier

Gaussian Naive Bayes classification on the **Social Network Ads** dataset — predicts whether a user purchases a product based on age and estimated salary.

## How It Works

1. Loads the Social Network Ads CSV (age, estimated salary, purchased label)
2. Splits data 75/25 into training and test sets
3. Applies feature scaling (standardisation)
4. Trains a **Gaussian Naive Bayes** classifier
5. Evaluates with a confusion matrix and plots decision boundaries for both sets

The classifier applies Bayes' theorem with a Gaussian likelihood assumption to compute posterior probabilities for each class, assigning the label with the highest probability.

## Dataset

`Social_Network_Ads.csv` — 400 records with columns: User ID, Gender, Age, Estimated Salary, Purchased (0/1).

## 🛠 Tech Stack

| | Tool | Purpose |
|---|---|---|
| 🐍 | Python 3 | Primary implementation |
| 📊 | R | Alternative implementation |
| 🤖 | scikit-learn | GaussianNB, train/test split, scaling |
| 📈 | matplotlib | Decision boundary visualisation |
| 🐼 | pandas / NumPy | Data loading and manipulation |
| 📦 | e1071 (R) | Naive Bayes in R |
| 📦 | caTools (R) | Train/test splitting in R |

## Getting Started

### Python

```bash
pip install numpy pandas matplotlib scikit-learn
python naive_bayes.py
```

### R

```r
install.packages(c("caTools", "e1071"))
source("naive_bayes.R")
```

## ⚠️ Known Issues

- **ElemStatLearn (R):** This package was removed from CRAN. The R visualisation section requires installing it from the CRAN archive or finding an alternative.
- The dataset CSV must be in the same directory as the script (Python resolves this automatically via `os.path`).
