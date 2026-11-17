# loan_approval_prediction_.ipynb
## AI Assistance and Learning Process

Artificial Intelligence tools were used during this project as learning and development assistants, particularly to help structure the machine learning methodology, understand certain technical concepts, troubleshoot code, and improve the overall project workflow.

The AI assistance was mainly focused on:
- Understanding and organizing the different stages of a machine learning project.
- Selecting and understanding appropriate preprocessing techniques.
- Understanding model selection and evaluation methods.
- Debugging code and clarifying technical concepts.
- Improving the documentation and presentation of the project.

The analysis, experimentation, interpretation of results, and learning process were part of my own work. I used AI as a support tool to strengthen my understanding of the machine learning workflow.

**My objective was not simply to obtain a working model, but to learn how a machine learning project is structured, developed, and evaluated in practice.**

# Loan Approval Prediction

## 1. Project Overview

This project focuses on predicting whether a loan application will be approved or rejected using machine learning.

Financial institutions receive numerous loan applications and must evaluate several factors before making lending decisions. Machine learning can help identify patterns in historical application data and support the analysis of loan approval decisions.

The objective of this project was to build a classification model capable of predicting loan approval outcomes based on applicant information.

## 2. Project Objectives

The main objectives were to:

- Explore and understand a real-world loan application dataset.
- Perform exploratory data analysis (EDA).
- Identify and handle missing values.
- Prepare numerical and categorical features for machine learning.
- Train a classification model.
- Evaluate the model's performance using appropriate metrics.
- Interpret the results and identify potential limitations.

## 3. Dataset

The project uses the Loan Prediction dataset from Kaggle.

The dataset contains information about loan applicants, including:

| Feature | Description |
|---|---|
| Gender | Applicant's gender |
| Married | Marital status |
| Dependents | Number of dependents |
| Education | Education level |
| Self_Employed | Self-employment status |
| ApplicantIncome | Applicant's income |
| CoapplicantIncome | Co-applicant's income |
| LoanAmount | Requested loan amount |
| Loan_Amount_Term | Loan repayment period |
| Credit_History | Credit history information |
| Property_Area | Property location category |
| Loan_Status | Loan approval outcome (target) |

The target variable is `Loan_Status`, which indicates whether a loan was approved (`Y`) or rejected (`N`).

## 4. Methodology

The project followed several machine learning stages.

### 4.1 Data Exploration

The dataset was initially explored using Pandas and data visualization libraries.

This stage included:
- Inspecting the dataset structure and data types.
- Identifying missing values.
- Analyzing numerical and categorical variables.
- Exploring relationships between applicant characteristics and loan approval outcomes.

### 4.2 Data Preprocessing

Data preprocessing was necessary to prepare the dataset for machine learning.

The main steps included:
- Handling missing values.
- Using median imputation for numerical variables.
- Using the most frequent value for categorical variables.
- Encoding categorical features into numerical representations.
- Scaling numerical features where appropriate.
- Separating the input features from the target variable.

### 4.3 Model Training

A Logistic Regression model was selected for this classification task.

Logistic Regression is a supervised machine learning algorithm commonly used for binary classification problems. It estimates the probability that an observation belongs to one of two classes.

The dataset was divided into training and testing sets to evaluate the model on data it had not used during training.

## 5. Model Evaluation

The model was evaluated using several classification metrics:

- **Accuracy:** Measures the overall proportion of correct predictions.
- **Precision:** Measures how many predicted cases in a class were correct.
- **Recall:** Measures how many actual cases in a class were correctly identified.
- **F1-score:** Combines precision and recall into a single metric.
- **Confusion Matrix:** Shows the distribution of correct and incorrect predictions.

### Results

The model achieved an accuracy of approximately **86.18%** on the test dataset.

The classification report showed different performance levels between the two classes:

| Metric | Rejected (0) | Approved (1) |
|---|---:|---:|
| Precision | 0.96 | 0.84 |
| Recall | 0.58 | 0.99 |
| F1-score | 0.72 | 0.91 |

These results indicate that the model performed particularly well at identifying approved applications. However, its recall for rejected applications was lower, meaning that some rejected applications were incorrectly classified.

This demonstrates why accuracy alone is not sufficient to evaluate a classification model.

## 6. Conclusion

This project provided practical experience with a complete machine learning classification workflow, from data exploration and preprocessing to model training and evaluation.

Although the model achieved an accuracy of approximately 86.18%, the evaluation revealed an imbalance in its ability to identify approved and rejected applications.

Further improvements could include:
- Testing other classification algorithms, such as Random Forest.
- Comparing different preprocessing strategies.
- Performing hyperparameter tuning.
- Investigating class imbalance and alternative evaluation metrics.

This project helped strengthen my understanding of supervised machine learning and its practical applications in financial decision-making.

## 7. AI Assistance and Transparency

AI tools were used throughout this project as learning and development assistants.

In particular, AI assistance helped me understand and organize the machine learning methodology, select appropriate preprocessing techniques, understand model evaluation metrics, troubleshoot code, and structure the project documentation.

I want to be transparent that I did not develop every methodological decision independently. AI played an important supporting role, especially in guiding the structure and methodology of the project.

My objective was to use this assistance as a learning opportunity, understand the different stages of a machine learning workflow, and gain practical experience working with data and predictive models.

## 8. Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook
