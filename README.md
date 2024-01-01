# credit-approval
A machine learning model to accurately predict the creditworthiness of customers

# Academic Project - Credit Scoring

## Author: Lakshman Palli

### Business Understanding
Banks and credit card companies face the challenge of determining the creditworthiness of individuals to minimize the risk of financial losses. Data mining is employed to analyze patterns and trends in customer data, aiding in better decision-making and reducing the likelihood of lending to high-risk individuals.

### Data Understanding
The dataset comprises 1000 entries with 21 columns, featuring both numerical and categorical attributes relevant to consumer credit risk assessment. The 'status' column serves as the target variable, indicating creditworthiness (Good: 1, Bad: 2).

### Data Preparation
1. **Isolation of Target Variable**: The 'status' variable was isolated.
2. **Dummy Variable Creation**: Categorical attributes were transformed into binary columns for modeling.
3. **Binary Labeling**: 'Good' (0) and 'Bad' (1) labels were assigned to the 'status' variable.
4. **Data Partitioning**: The dataset was split into a 90-10 training-testing set.
5. **Scaling**: StandardScaler was used to standardize the data for equal contribution in algorithms.
6. **Feature Selection**: RandomForestClassifier aided in selecting 35 features based on importance scores.

### Modeling
Two models were employed: Logistic Regression and Random Forest Classifier.

#### Logistic Regression Results:
- **Accuracy**: 78%
- **Precision, Recall, F1-Score (Bad Credits)**: 0.62, indicating balanced performance.

#### Random Forest Classifier Results:
- **Accuracy**: 72%
- **Precision, Recall (Bad Credits)**: Lower than Logistic Regression.

#### Hyperparameter Tuning:
- GridSearchCV tuned Logistic Regression hyperparameters with no change in accuracy.

#### Visualizations:
1. **Confusion Matrix**: Identified model mistakes (11 false positives, 11 false negatives).
2. **ROC Curve**: Balanced true positive and false positive rates.
3. **Precision-Recall Curve**: Balanced trade-off between precision and recall.

### Conclusion on Modeling
Logistic Regression demonstrated more balanced performance. Hyperparameter tuning refined the model. Visualizations highlighted areas for improvement.

### Evaluations
- **False Positives and Negatives**: Both present, requiring careful consideration.
- **Precision and Recall**: Balanced, crucial for business success.
- **Robustness**: Further evaluation needed for diverse customer profiles and economic changes.

### Deployment
#### Benefits:
- **Automated Decision-Making**: Efficient credit scoring process.
- **Risk Mitigation**: Identifying potential bad loans, reducing bad debt.

#### Concerns and Issues:
- **Model Interpretability**: Stakeholder understanding and trust are crucial.
- **Data Privacy and Ethics**: Secure and ethical handling of customer data.
- **Changing Economic Environments**: Continuous monitoring and tuning required.

### Wisdom from the Project
1. **Importance of Data Preparation**: Vital for improving model performance.
2. **Model Evaluation**: Holistic evaluation beyond accuracy is essential.
3. **Continuous Improvement**: Ongoing monitoring, evaluation, and improvement are necessary for adapting to evolving conditions and enhancing decision-making.
