# Customer-Churn-Prediction

## 🔧 Preprocessing Steps

1. **Data Cleaning**:
   - Removed non-predictive columns: `RowNumber`, `CustomerId`, `Surname`
   - Zero missing values found in dataset

2. **Feature Engineering**:
   - Label Encoded: `Gender` (Female:0, Male:1)
   - One-Hot Encoded: `Geography` (with drop_first=True)
   - Standard Scaled all numerical features

## 🤖 Model Selection

**Random Forest Classifier** was implemented with:
- 100 estimators (n_estimators=100)
- Default hyperparameters
- Random state fixed (42) for reproducibility

## 📊 Performance Analysis

### Key Metrics:

| Metric       | Score  |
|--------------|--------|
| Accuracy     | 0.86   |
| Precision    | 0.78   |
| Recall       | 0.43   |
| F1 Score     | 0.55   |
| ROC AUC      | 0.84   |

### Visualizations:
- Confusion Matrix
- ROC Curve (AUC = 0.84)
- Feature Importance Plot
- Class Distribution Chart

