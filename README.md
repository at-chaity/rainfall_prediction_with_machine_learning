# rainfall_prediction_with_machine_learning

This mini project uses historical Australian weather data to predict whether it will rain tomorrow, based on various meteorological factors.

## 🔍 Dataset
- Source: [Rain in Australia - Kaggle](https://www.kaggle.com/jsphyg/weather-dataset-rattle-package)
- Size: ~145,000 records, 23 features (reduced after cleaning)

## 🧹 Process Overview
- Removed rows with excessive missing data
- Converted binary labels (`Yes`/`No`) to numeric (`1`/`0`)
- Encoded categorical columns using Label Encoding
- Filled missing numeric values with median
- Dropped non-informative features like `Date` and `Location`

## 🧠 Model
- Algorithm: `RandomForestClassifier`
- Train/Test Split: 80/20
- Achieved Accuracy: **~85.8%**

## 📊 Evaluation
- Confusion Matrix:
  - ✅ Correct No Rain: 20,621
  - ✅ Correct Rain: 3,148
  - ❌ Missed Rain: 2,997
  - ❌ False Alarm: 935
- Top Predictor: **Humidity at 3PM**
  - Boxplot analysis confirms higher humidity increases rain likelihood

## 🛠️ Tools Used
- Python
- `pandas`, `matplotlib`, `seaborn`, `scikit-learn`

## 📁 Files Included
- `Rainfall_Prediction.ipynb` — Jupyter notebook with all code, plots, and output
- `README.md` — This file

---

📌 A clean and simple ML classification example with real-world relevance.
