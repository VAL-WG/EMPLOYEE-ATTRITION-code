OVERVIEW
Predicting employee attrition is crucial for organizations to proactively manage human resources and retain talent.  
This project uses machine learning to predict whether an employee is likely to leave the company based on demographic, work, and performance data.

Dataset: WA_Fn-UseC_-HR-Employee-Attrition.csv (1,470 records, 35 features)  

Goal: Identify employees at risk of leaving to support HR decision-making and improve retention strategies.

---

1. Project Workflow

  Introduction & Data Collection
  - Loaded and explored the dataset.  
  - Examined structure, data types, and sample records to understand employee information.

  Data Exploration & Cleaning
  - Checked for missing values (none found).  
  - Analyzed numerical distributions and visualized key features to understand patterns.  

  Feature Engineering & Selection
  - Removed irrelevant columns.  
  - Created new features:
        PromotionGap: Time since last promotion.  
        WorkloadPressure: Job level × overtime status to estimate stress.  
  - Encoded categorical variables for model training.
  
  Model Building
  - Split data into features and target variable.  
  - Created training and testing sets.  
  - Trained a **Logistic Regression** model to predict employee attrition.

  Model Evaluation
  - Evaluated the model using Accuracy, Precision, Recall, F1 Score, and Confusion Matrix.  
    Results:
    - Accuracy: 87%  
    - Precision (Left): 56%  
    - Recall (Left): 26%  
    - F1 Score (Left): 35%  
  - Model performs well in identifying employees who stay, but has room for improvement in predicting departures.

2. Tools & Libraries
- Python 3 
- Pandas & NumPy – Data manipulation  
- Seaborn & Matplotlib – Data visualization  
- Scikit-learn – Machine learning
  
3. Future Improvements
- Scale numerical features to improve model performance.  
- Experiment with other models like Random Forest and XGBoost.  
- Perform feature importance analysis to identify key drivers of attrition.


