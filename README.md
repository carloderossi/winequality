# Wine Quality Classification Project

## Overview

This project focuses on classifying the quality of wine based on various chemical properties. The dataset used in this project contains several features that describe the chemical composition of different wine samples, and the target variable is the quality of the wine.

## Dataset

The dataset contains the following features:
- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol
- Quality (Target variable)

## Objective

The objective of this project is to build a classification model that can accurately predict the quality of wine based on its chemical properties.

## Approach

1. **Data Preprocessing**:
   - Handling missing values
   - Data normalization
   - Feature selection
   - Splitting the dataset into training and testing sets

2. **Exploratory Data Analysis (EDA)**:
   - Analyzing the distribution of features
   - Identifying correlations between features and the target variable
   - Visualizing the data using various plots

3. **Model Building**:
   - Training multiple classification models such as:
     - Logistic Regression
     - Decision Tree Classifier
     - Random Forest Classifier
     - Support Vector Machine (SVM)
   - Evaluating model performance using metrics such as accuracy, precision, recall, and F1-score

4. **Model Evaluation**:
   - Comparing the performance of different models
   - Selecting the best-performing model based on evaluation metrics
   - Fine-tuning the selected model for optimal performance

## Results

The results section will include:
- Performance metrics for each model
- Confusion matrix for the best-performing model
- ROC curve and AUC score for the best-performing model
- Feature importance analysis

### Conclusion

**Random Forest Classifier:**
- Cross-Validation F1 Score: 0.9335 (Excellent performance)
- **Classification Report:**
  - **Class 0**: Precision, Recall, F1-Score are 0.00 (poor prediction, likely due to very few samples)
  - **Class 1**: Precision (0.91), Recall (0.98), F1-Score (0.95) (well predicted)
  - **Class 2**: Precision (0.84), Recall (0.57), F1-Score (0.68) (moderately well predicted)
- Accuracy: 0.91
- Macro Average F1-Score: 0.54 (reflects poor performance for minority class)
- Weighted Average F1-Score: 0.89

**Gradient Boosting Classifier:**
- Cross-Validation F1 Score: 0.8957 (high, but slightly lower than Random Forest)
- **Classification Report:**
  - **Class 0**: Precision, Recall, F1-Score are 0.00 (poor prediction, likely due to very few samples)
  - **Class 1**: Precision (0.94), Recall (0.82), F1-Score (0.87) (well predicted)
  - **Class 2**: Precision (0.45), Recall (0.82), F1-Score (0.58) (moderately well predicted)
- Accuracy: 0.80
- Macro Average F1-Score: 0.49 (reflects poor performance for minority class)
- Weighted Average F1-Score: 0.82

### Insights and Recommendations

**Performance:**
- Both models show high overall performance.
- Random Forest slightly outperforms Gradient Boosting in F1 score and accuracy.

**Class Imbalance Impact:**
- Class 0 is poorly predicted by both models, likely due to the small sample size.
- Further balancing techniques or additional data for this class are needed.

**Model Choice:**
- Random Forest Classifier is recommended due to its higher F1 score and robustness in handling imbalanced data.

### Next Steps

**Further Class Balancing:**
- Explore techniques to handle class imbalance for Class 0, such as SMOTE or synthetic data generation.
- Consider collecting more data for the underrepresented class.

**Hyperparameter Tuning:**
- Fine-tune hyperparameters for both Random Forest and Gradient Boosting to improve performance.

**Ensemble Methods:**
- Explore combining predictions from multiple models to improve performance, particularly for the minority class.

**Feature Engineering:**
- Continue experimenting with feature engineering techniques to uncover more predictive patterns in the data.


## References

- [Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)

## Author

Carlo De Rossi
