
# Job Applicant Success Prediction
![DecisionTree_2](https://github.com/user-attachments/assets/3c58533f-0547-42fb-b194-39b6f6ec9a3b)

## 📖 Project Overview
This project involves building a Decision Tree model to predict the likelihood of job applicants succeeding in a specific role. The dataset, sourced from [Kaggle](https://www.kaggle.com/datasets/ayushtankha/70k-job-applicants-data-human-resource/data), contains information on over 70,000 applicants, including demographic, educational, and professional attributes.  

The goal is to classify candidates as either "Successful" or "Unsuccessful" based on their attributes using Python and machine learning techniques.

## 🎯 Features
The dataset includes the following features:  
- **Age:** Applicant’s age categorized as >35 or ≤35.  
- **Education Level (EdLevel):** Highest level of education (e.g., Undergraduate, Master, PhD).  
- **Gender:** Applicant’s gender (e.g., Man, Woman, Non-Binary).  
- **Accessibility:** Whether the applicant has any accessibility requirements.  
- **Main Branch:** Whether the applicant is a professional developer.  
- **Years of Coding Experience (YearsCode):** Total years of coding experience.  
- **Professional Coding Experience (YearsCodePro):** Years coding in a professional setting.  
- **Previous Salary:** Applicant’s last known salary.  
- **Computer Skills:** Number of technical skills the applicant possesses.  
- **Target Variable:** Whether the applicant is **Employed (1)** or **Not Employed (0)**.

## 📊 Project Workflow
### 1. Data Preprocessing
- Cleaned the dataset by dropping redundant columns: `Unnamed: 0`, `Employment`, `Country`, and `HaveWorkedWith`.  
- Handled missing values and applied label encoding to categorical variables using custom mappings for Age, Gender, Education Level, and Accessibility.

### 2. Model Development
- Built a Decision Tree Classifier using Gini impurity as the splitting criterion.  
- Set a maximum tree depth of 3 to prevent overfitting.  
- Split data into training (70%) and testing (30%) sets.  

### 3. Hyperparameter Tuning
- Performed Grid Search with cross-validation to optimize parameters (`max_depth`, `min_samples_split`, and `min_samples_leaf`).  

### 4. Visualization
- Visualized the trained Decision Tree using **Graphviz** and exported the graph as `.dot` and `.jpg` files.  

### 5. Model Evaluation
- Measured model performance using accuracy, precision, and recall metrics.

  

## 🙏 Acknowledgments
- **Dataset:** The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/ayushtankha/70k-job-applicants-data-human-resource/data).  
