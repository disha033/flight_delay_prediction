
# ✈️ Flight Delay Prediction Project

## 📝 Project Description
Predicting 60+ minute flight delays using XGBoost machine learning model. This project analyzes historical flight data to identify patterns and build a predictive model for flight delays.

## 📋 Table of Contents
- [Features](#-features)
- [Installation](#-installation)
- [Dataset](#-dataset)
- [Methodology](#-methodology)
- [Results](#-results)
- [Future Improvements](#-future-improvements)

## 🌟 Features
- Data cleaning and preprocessing pipeline
- Exploratory Data Analysis (EDA)
- XGBoost classification model
- Hyperparameter tuning with GridSearchCV
- Performance evaluation metrics

## 💻 Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/flight-delay-prediction.git
cd flight-delay-prediction
```

2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
```

## 📂 Dataset
The dataset contains:
- **Features**: DayOfWeek, DepTime, Airline, Origin, Dest
- **Target**: `is_delayed_60+` (1 if CarrierDelay > 60 minutes)

**Preprocessing steps**:
- Date feature extraction (month/day)
- One-hot encoding for categorical variables

## 🔬 Methodology
1. **Data Analysis**:
   - Class imbalance handling (7.46% positive cases)
   - Delay pattern analysis by day/airline/airport

2. **Modeling**:
   - Baseline XGBoost classifier
   - Hyperparameter tuning with GridSearchCV

3. **Evaluation Metrics**:
   - Accuracy
   - AUC-ROC
   - Confusion matrix

## 📊 Results
### Baseline Model
- Accuracy: 92.46%
- AUC-ROC: 0.7095

### Tuned Model (Best Parameters)
| Parameter       | Value |
|----------------|-------|
| learning_rate  | 0.2   |
| max_depth      | 7     |
| n_estimators   | 250   |
| subsample      | 1.0   |

**Improved Performance**:
- Accuracy: 92.49% (+0.03%)
- AUC-ROC: 0.7206

## 🚀 Future Improvements
- Address class imbalance with advanced techniques
- Incorporate weather data
- Feature importance analysis
- Model deployment as web service

