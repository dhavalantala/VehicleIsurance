# 🚗 Vehicle Insurance Cross-Sell Prediction

A machine learning project that predicts whether an existing **health insurance customer** is likely to purchase **vehicle insurance** — helping insurance companies prioritise outreach and improve conversion rates.

---

## 📌 Problem Statement

Insurance companies spend heavily on customer acquisition. This project builds a binary classifier to identify which customers are most likely to respond positively to a vehicle insurance offer, enabling smarter, targeted campaigns.

**Target variable:** `Response` — `1` (Interested) / `0` (Not Interested)

---

## 📂 Dataset Features

| Feature | Description |
|---|---|
| `Age` | Age of the customer |
| `Gender` | Male / Female |
| `Driving_License` | 1 = Has licence, 0 = Does not |
| `Region_Code` | Anonymised region of the customer |
| `Previously_Insured` | 1 = Already has vehicle insurance, 0 = Does not |
| `Vehicle_Age` | Age of the vehicle (< 1 Year / 1–2 Years / > 2 Years) |
| `Vehicle_Damage` | 1 = Vehicle was damaged in the past, 0 = Was not |
| `Annual_Premium` | Amount paid per year for health insurance |
| `Policy_Sales_Channel` | Anonymised outreach channel (agent, mail, phone, etc.) |
| `Vintage` | Days the customer has been associated with the company |
| `Response` | **Target** — 1 = Interested, 0 = Not Interested |

---

## 📊 Results & Model Performance

**Model:** Random Forest Classifier (tuned via `RandomizedSearchCV`)

**Best Hyperparameters:**
- `n_estimators`: 300
- `criterion`: entropy
- `max_depth`: 10
- `min_samples_split`: 7
- `min_samples_leaf`: 6

| Metric | Class 0 (Not Interested) | Class 1 (Interested) |
|---|---|---|
| Precision | 0.88 | 0.85 |
| Recall | 0.90 | 0.83 |
| F1 Score | 0.89 | 0.84 |
| **Accuracy** | **87%** | |

> 📄 [View the Full Interactive Report →](https://yourusername.github.io/your-repo-name)

---

## 🛠️ Tech Stack

`Python` · `pandas` · `scikit-learn` · `seaborn` · `matplotlib` · `imbalanced-learn`
