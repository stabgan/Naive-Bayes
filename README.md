# 🧠 Naive Bayes Classification

A binary classification project using the **Gaussian Naive Bayes** algorithm to predict whether a user will purchase a product based on their age and estimated salary. Implementations provided in both Python and R.

---

## 📖 Methodology

This project applies the **Gaussian Naive Bayes** classifier — a probabilistic model grounded in **Bayes' Theorem**:

```
P(class | features) = P(features | class) × P(class) / P(features)
```

The pipeline follows these steps:

1. **Load** the `Social_Network_Ads.csv` dataset (age, estimated salary → purchased).
2. **Split** into 75 % training / 25 % test sets.
3. **Scale** features with `StandardScaler` (Python) or `scale()` (R).
4. **Train** a Gaussian Naive Bayes model on the training set.
5. **Evaluate** with a confusion matrix and decision-boundary visualisations.

---

## 🛠️ Tech Stack

| Layer | Tool |
|-------|------|
| 🐍 Language | Python 3 |
| 📊 Language | R |
| 🤖 ML Framework | scikit-learn |
| 📈 Visualisation | matplotlib · ElemStatLearn |
| 🗃️ Data Handling | pandas · NumPy |

---

## 📦 Dependencies

### Python

```
numpy
pandas
matplotlib
scikit-learn
```

Install with:

```bash
pip install numpy pandas matplotlib scikit-learn
```

### R

```r
install.packages(c("caTools", "e1071"))
# ElemStatLearn has been removed from CRAN — see Known Issues
```

---

## 🚀 How to Run

### Python

```bash
cd Naive-Bayes
python naive_bayes.py
```

The script prints the confusion matrix and opens two matplotlib windows showing the decision boundaries for the training and test sets.

### R

```r
source("naive_bayes.R")
```

Or run interactively in RStudio.

---

## ⚠️ Known Issues

| # | Issue | Details |
|---|-------|---------|
| 1 | `ElemStatLearn` removed from CRAN | The R visualisation section depends on `ElemStatLearn`, which was archived. Install from the CRAN archive or a mirror, or comment out the visualisation block. |
| 2 | Matplotlib GUI backend required | `plt.show()` needs an interactive backend (e.g. TkAgg). In headless environments, switch to `Agg` and save figures to files instead. |

---

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.
