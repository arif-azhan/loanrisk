# Loan Risk Prediction (End to End Data Science Workflow and ML Model Deployment)

## Objective
The goal of this project is to predict the likelihood of loan repayment using datasets related to loans, payments, and underwriting variables. The project focuses on data cleaning, exploratory data analysis (EDA), feature engineering, and the development of machine learning models to classify loan applicants as "High Risk" or "Low Risk."

---

## Project Structure
1. **Data Cleaning and Preparation**:
   - Examined datasets for missing values and inconsistencies.
   - Cleaned and prepared data for analysis.
   - Handled missing values using techniques such as imputation and removal of unreliable data.

2. **Feature Engineering**:
   - Created meaningful features from historical payment behavior and underwriting variables.
   - Established a binary classification label (`risk_flag`) to indicate "High Risk" or "Low Risk" applicants.

3. **Model Development and Evaluation**:
   - Built and evaluated models using:
     - K-Nearest Neighbors (k-NN)
     - Decision Tree Classifier
   - Evaluated models with metrics like accuracy, confusion matrices, and classification reports.

4. **Exploratory Data Analysis (EDA)**:
   - Analyzed distributions and relationships between variables.
   - Visualized patterns and correlations to identify significant predictors.

5. **Conclusion and Future Work**:
   - Addressed overfitting concerns and proposed solutions like dimensionality reduction (PCA) and hyperparameter tuning.
   - Identified areas for future analysis, such as incorporating late payment behavior and scheduling.

---

## Datasets Used
1. **Loan Data**: Contains loan-related details such as loan amounts, APR, and loan status.
2. **Payment Data**: Contains historical payment information, including statuses and payment amounts.
3. **Clarity Underwriting Data**: Includes fraud scores and underwriting variables.

---

## Key Features
- **`missed_payment`**: Indicates whether an applicant has a rejected payment.
- **`missed_payments_count`**: Total number of missed payments per applicant.
- **`risk_flag`**: A binary classification label (High Risk or Low Risk) based on payment behavior.

---

## Results

### Model Performance
- **k-Nearest Neighbors (k-NN)**:
  - Accuracy: 100%
  - Strength: Effective at identifying low-risk applicants.
  - Concern: Potential overfitting due to high accuracy.

- **Decision Tree**:
  - Accuracy: 100%
  - Strength: Successfully identified high-risk applicants.
  - Concern: Slightly higher false-negative count compared to k-NN.

### Insights from EDA
- Applicants with higher loan amounts tend to have lower APRs.
- A positive correlation exists between principal and payment amounts.
- Fraud scores are higher for low-risk applicants.

---

## Tools and Libraries Used
- **Python Libraries**: 
  - Data manipulation: `pandas`, `numpy`
  - Data visualization: `matplotlib`, `seaborn`
  - Machine learning: `scikit-learn`

---

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/arif-azhan/loanrisk.git
