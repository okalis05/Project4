## project 4
---
## Predicting The 2024 Presidential Election outcome with Machine Learning algorithms
---

### Overview

This project aims to predict the outcome of the 2024 US Presidential Elections . By leveraging historical data from previous elections (2000-2020), economic indicators, demographic information, and campaign finance data, we have developed machine learning models to forecast election results. The primary goal is to create accurate predictions while addressing challenges such as data imbalance and model bias.

### Project Objectives
- Objective:Predict the winner of the 2024 presidential elections.
- Prediction Type:Binary classification (e.g., Candidate A vs. Candidate B).

### Technologies Used
- Machine Learning Libraries:Scikit-learn, TensorFlow
- Data Processing:Python Pandas
- Data Visualization:Python Matplotlib 


### Data Collection
- `Elections results data` from 'kaggle'
- `Demographic data` from the 'US Census Bureau'
- `Economic Indicators data` with aggregated financial information from election campaigns, including contributions, loans, disbursements,
   and expenditures imported from the 'Federal Election Commission (FEC)' database
- `Pollind data` from 'FiveThirtyEight'

### Data Preprocessing
- Cleaning: Handled missing values, removed duplicates, and corrected inconsistencies in the dataset.
- Feature Engineering: Created new features, such as sentiment scores from social media posts and changes in economic indicators, to enhance model prediction.
- Normalization: Scaled numerical data to ensure all features contributed equally to the model.

### Model Development
Three primary models were developed and evaluated:

#### 1. Random Forest Classifier
- Preprocessing: Data scaling, feature selection
- Performance: High overall accuracy (95%), but limited ability to predict winners (32% accuracy due to data imbalance)
- Feature Importance: Financial contributions and expenditures were the most significant features influencing election outcomes.

#### 2. Logistic Regression
   - Preprocessing: Similar to Random Forest
   - Performance: Similar accuracy in predicting losers (96%), but struggled with predicting winners (23% accuracy)
   
#### 3. Neural Network
   - Objective: To explore deep learning methods for potentially higher accuracy.
   - Keras_tuner to optimize the neural network model to achieve even higher accuracy

### Model Evaluation
- Metrics Used: Accuracy, precision, recall, F1 score, and ROC-AUC.
- Insights: The imbalance in the data led to high accuracy in predicting losing candidates but poor performance in predicting winners. This highlights the need for addressing data imbalance in future iterations.

### Model Deployment
- Real-Time Predictions: A system is set up to collect real-time data and update predictions as new information becomes available.
- Monitoring: Continuous monitoring of the model's performance is essential, with plans to update and refine the model as necessary.

### Ethical Considerations
- Bias Mitigation: Ensured that the model does not perpetuate or amplify biases present in the data by applying various bias mitigation techniques during preprocessing and evaluation.

### Conclusion
The models developed in this project demonstrated high overall accuracy but faced challenges in predicting actual winners due to data imbalance. Future work will focus on addressing these imbalances and exploring additional models and techniques to improve prediction accuracy for the 2024 election.

### Contributors
- Elis Okala 
- Monique Reid 


