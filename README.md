## Heart Disease Classification

### Problem
Early detection of heart disease can significantly improve patient outcomes.  
This project applies machine learning models to classify the presence of heart disease using clinical patient data.

### Data
- 303 patient records
- 14 clinical features including age, cholesterol, chest pain type, maximum heart rate, and exercise-induced angina
- Target variable: heart disease presence (0 = No, 1 = Yes)

### Approach
- Performed exploratory data analysis and correlation analysis
- Removed outliers from numeric features using Tukey’s IQR method
- Applied feature selection based on correlation insights
- Trained and compared multiple models:
  - Logistic Regression
  - K-Nearest Neighbors (K selected using learning curves)
  - Support Vector Machine (RBF kernel)
  - Random Forest
  - Ensemble Voting

### Evaluation
Models were evaluated using:
- Accuracy
- ROC-AUC
- Precision and Recall
- Confusion Matrices

Logistic Regression achieved the highest ROC-AUC, providing strong class separation while remaining interpretable and robust.

### Key Learnings
- Model performance should be evaluated using multiple metrics, not accuracy alone
- Simpler, well-evaluated models can outperform more complex approaches
- ROC-AUC is particularly important for healthcare-related classification tasks

### Limitations & Next Steps
- Expand the dataset to improve generalization
- Explore additional feature engineering
- Validate models on external or more diverse patient populations
