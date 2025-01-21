# Predicting Hospital Readmissions

This project is part of a **Big Data and Data Analytics Course** and aims to address the challenge of hospital readmissions, a critical issue in healthcare management. This README provides detailed information on the problem, solution, implementation, and results of the project.

---

## **Problem Statement**

Hospital readmissions within 30 days of discharge are a major concern in the healthcare industry. They increase patient risk, disrupt treatment continuity, and impose significant costs on healthcare systems. Identifying patients at risk of readmission can enable timely interventions and improve patient outcomes.

---

## **Solution Description**

This project leverages **machine learning techniques** to predict whether a patient is likely to be readmitted within 30 days of their initial discharge. The solution is designed to:
- Analyze patient data (e.g., demographics, medical history, and test results).
- Provide healthcare professionals with actionable insights for proactive interventions.
- Optimize resource allocation and reduce readmission rates.

### **Key Features**
- **Interactive Web App**: Built with Streamlit, the application allows users to input patient details and receive predictions on readmission likelihood.
- **Customizable Inputs**: Users can specify variables such as gender, admission type, diagnosis, lab procedures, and medication counts.
- **Accurate Predictions**: The model utilizes patient data to classify whether readmission is required or not.

---

## **Implementation Details**

1. **Data Preprocessing**:
   - The model was trained on healthcare datasets containing information on patient demographics, diagnoses, procedures, and previous hospital visits.
   - Missing values were imputed, and categorical variables were encoded for machine learning compatibility.

2. **Model Training**:
   - A supervised learning approach was used, and multiple algorithms (e.g., Logistic Regression, Random Forest, Gradient Boosting) were tested.
   - The best-performing model was saved as a `.pkl` file for deployment.

3. **Web Application**:
   - The Streamlit framework is used for a user-friendly interface.
   - Inputs are processed and passed to the trained model to generate predictions.


---

## **Main Technologies Used**

- **Programming Languages**: Python
- **Machine Learning Techniques**:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
- **Libraries and Tools**:
  - **Streamlit**: For creating the interactive web application.
  - **Scikit-learn**: For model development and evaluation.
  - **Pandas & NumPy**: For data manipulation and preprocessing.


---

## **Results**

- **Model Performance**:
  - Achieved an accuracy of **85%** and an AUC-ROC score of **0.89** on test data.
  - Feature importance analysis identified key predictors, such as:
    - **Number of inpatient visits**
    - **A1C results**
    - **Admission type**

- **Application Usability**:
  - A streamlined interface for healthcare professionals to input patient details and receive instant predictions.
  - Proactive identification of high-risk patients enables better care management and reduced readmission rates.

