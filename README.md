# Predicting Hospital Readmissions: README

This project is part of a **Data Analytics Course** and aims to address the issue of hospital readmissions. By employing advanced machine learning techniques, the project predicts whether a patient will require readmission within 30 days of discharge. Below is a detailed overview of the project, its implementation, and results.

---

## **Problem Statement**

Hospital readmissions within 30 days of discharge are a pressing concern. They lead to higher costs, overburdened healthcare systems, and increased patient risks. Predicting the likelihood of readmission can help healthcare providers proactively manage high-risk patients and improve care quality.

---

## **Solution Description**

This project develops a machine learning model to predict hospital readmissions. The solution:
- Processes patient demographic and clinical data.
- Provides predictions on whether readmission is required.
- Helps healthcare providers take timely, preventive measures.

### **Key Features**
- **Comprehensive Analysis**: Utilizes patient information such as medical history, lab results, and previous visits.
- **Interactive Web Application**: Built using Streamlit, it offers an intuitive interface for entering patient data and obtaining predictions.
- **Actionable Insights**: Enables proactive interventions to reduce readmission rates.

---

## **Implementation Details**

### **Tasks Completed**

1. **Data Preprocessing**:
   - Handled outliers and skewed data distributions.
   - Performed feature selection using heatmaps and variance inflation factor (VIF) analysis.

2. **Feature Engineering**:
   - Developed a separate notebook for predicting A1C values to enrich the dataset.
   - Engineered new features to enhance model performance.

3. **Model Building**:
   - Tried various machine learning models, including:
     - Logistic Regression
     - Support Vector Classifier (SVC)
     - Decision Tree Classifier
     - Random Forest Classifier
     - XGBoost Classifier
   - Chose the best-performing model based on accuracy and AUC metrics.

4. **Handling Imbalanced Data**:
   - Used the **SMOTE-Tomek** method to address class imbalance in the dataset.

5. **Model Evaluation**:
   - Evaluated performance using cross-validation, confusion matrix, classification report, and AUC metrics.

---

## **Main Technologies Used**

- **Programming Languages**: Python
- **Libraries**:
  - **Data Manipulation**: pandas, numpy
  - **Visualization**: matplotlib, seaborn
  - **Modeling and Evaluation**: scikit-learn, XGBoost, imbalanced-learn (for SMOTE-Tomek)

---

## **Results**

### **Performance Metrics**

- **Accuracy**:
  - Train Accuracy: **89.38%**
  - Test Accuracy: **91.00%**

- **Confusion Matrix**:
  ```
  [[99 17]
   [ 1 83]]
  ```

- **Classification Report**:
  ```
                precision    recall  f1-score   support

             0       0.99      0.85      0.92       116
             1       0.83      0.99      0.90        84

      accuracy                           0.91       200
     macro avg       0.91      0.92      0.91       200
  weighted avg       0.92      0.91      0.91       200
  ```

- **Receiver Operating Characteristic (ROC) Curve**:
  - False Positive Rate: `[0.0, 0.1465, 1.0]`
  - True Positive Rate: `[0.0, 0.988, 1.0]`
  - Thresholds: `[inf, 1.0, 0.0]`

- **Area Under the Curve (AUC)**:
  - **0.921**

