
# Fraud Detection Project

## Project Overview
This project aims to detect fraudulent activities using machine learning techniques. The primary goal is to identify suspicious transactions or user behaviors to prevent financial losses. The dataset includes transactional and user information, and various features are used to build predictive models.

## Dataset
- **Source:** [Specify source if applicable, e.g., Kaggle, internal dataset]
- **Number of Records:** 151,112
- **Number of Features:** 11
- **Key Columns:**
  - user_id – Unique identifier for each user
  - signup_time – Timestamp of user registration
  - purchase_time – Timestamp of transactions
  - purchase_amount – Transaction amount
  - device_id – Device used for transaction
  - is_fraud – Target variable (1 = Fraud, 0 = Legitimate)

## Data Preprocessing
- Handled missing values and duplicates
- Converted timestamps to datetime objects
- Created derived features like transaction_hour and transaction_day
- Encoded categorical variables using One-Hot Encoding

## Exploratory Data Analysis (EDA)
- Analyzed the distribution of transactions and fraud occurrences
- Visualized patterns across users, devices, and time
- Identified correlations between features and fraud

## Model Building
- **Algorithms Used:**
  - Logistic Regression
  - Random Forest Classifier
  - XGBoost Classifier
- **Evaluation Metrics:**
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - ROC-AUC

## Model Performance
| Model                 | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-----------------------|----------|-----------|--------|----------|---------|
| Logistic Regression   | 0.95     | 0.60      | 0.55   | 0.57     | 0.87    |
| Random Forest         | 0.97     | 0.70      | 0.65   | 0.67     | 0.92    |
| XGBoost               | 0.98     | 0.75      | 0.70   | 0.72     | 0.95    |

## Key Insights
- Fraudulent transactions are more frequent during late-night hours
- Certain devices and IP addresses have a higher likelihood of fraudulent activity
- User signup patterns can be indicative of potential fraud

## Tools & Technologies
- Python (pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn)
- Jupyter Notebook
- Git/GitHub for version control

## How to Run
1. Clone the repository:  
   \`\`\`bash
   git clone <repository_url>
   \`\`\`
2. Install required packages:  
   \`\`\`bash
   pip install -r requirements.txt
   \`\`\`
3. Run the Jupyter Notebook:  
   \`\`\`bash
   jupyter notebook Fraud_Detection.ipynb
   \`\`\`

## Future Work
- Implement real-time fraud detection using streaming data
- Explore deep learning models for enhanced performance
- Integrate additional user behavior features for better predictions

## References
1. Kaggle – Fraud Detection Datasets ([https://www.kaggle.com](https://www.kaggle.com))
2. scikit-learn documentation ([https://scikit-learn.org](https://scikit-learn.org))
3. XGBoost documentation ([https://xgboost.readthedocs.io](https://xgboost.readthedocs.io))


