# Patient Appointment No-Show Prediction

## Project Overview
Machine Learning model to predict whether a patient will attend or miss their scheduled medical appointment.

## Dataset
- Source: Brazilian Hospital (Kaggle)
- Records: 110,527 appointments
- Features: Patient demographics, medical conditions, appointment details

## Methodology
1. Data Cleaning (removed negative age, fixed spelling, Converted Data Columns)
2. Feature Engineering (WaitingDays)
3. EDA (Age vs No-Show, Class Imbalance analysis)
4. Model Training (Logistic Regression, Random Forest, XGBoost)
5. Evaluation (Accuracy, Precision, Recall, F1, ROC-AUC)

## Results
| Model | Accuracy | No-Show Recall | AUC |
|-------|----------|----------------|-----|
| Logistic Regression | 66.37% | 56% | 0.664 |
| Random Forest | 69.57% | 42% | 0.636 |
| **XGBoost** | **59.74%** | **78%** | **0.720** |

## Best Model: XGBoost
- Highest AUC: 0.72
- Catches 78% of actual no-shows
- Most important feature: WaitingDays (46% importance)

## Key Recommendations
1. Reduce waiting time (same-day/next-day scheduling)
2. Send SMS reminders
3. Extra attention to young adults (18-35)
4. Overbook high-risk appointment slots

## Files
- `no_show_prediction.ipynb` - Main notebook
- `KaggleV2-May-2016.csv` - Dataset 

## Author
[Your Name]
