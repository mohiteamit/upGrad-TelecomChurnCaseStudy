# upGrad - Telecom Churn Prediction Project

## Overview
This project aims to predict customer churn in a telecom company using various machine learning models. The notebook explores several data preprocessing steps, feature selection techniques, and model evaluation approaches to identify customers who are likely to leave the service.

## Dataset
The dataset used for this project includes historical data of telecom customers, such as call minutes, recharge amounts, and usage statistics over several months. The target variable is `churn_probability`, indicating whether a customer is likely to churn (1) or not (0).

## Steps in the Notebook
1. **Data Loading and Cleaning**:
   - Loaded the dataset and performed initial exploratory data analysis (EDA).
   - Cleaned data by handling missing values and removing redundant or less informative features.

2. **Feature Engineering**:
   - Created additional features based on existing columns to derive more insights.
   - Employed quantile-based thresholds to identify high-value customers.

3. **Feature Selection**:
   - Used Recursive Feature Elimination (RFE) and Principal Component Analysis (PCA) to select important features.
   - Top 20 features selected by RFE include 'total_ic_mou_8', 'total_rech_amt_8', 'vol_2g_mb_8', etc.

4. **Data Splitting**:
   - Split the data into training and testing sets, ensuring the same proportion of churn and non-churn customers in both sets.

5. **Model Building**:
   - Tested multiple machine learning models, including Logistic Regression, Decision Trees, RandomForest, and XGBoost, with a combination of RFE and PCA for feature reduction.
   - Hyperparameter tuning was performed using GridSearchCV to optimize each model's performance.

6. **Evaluation**:
   - Evaluated model performance using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.
   - Plotted ROC curves for each model to visualize their ability to distinguish between churn and non-churn customers.

7. **Results**:
   - Compared different models, and discussed their strengths and weaknesses in predicting churn cases, especially focusing on the minority churn class.

## Key Insights
- **Feature Selection**: Feature engineering and RFE helped narrow down to the most impactful features, improving model interpretability.
- **Model Performance**: RandomForest performed the best with high accuracy, recall, and AUC, effectively distinguishing between churn and non-churn customers.
- **Challenges**: The main challenge was dealing with class imbalance, which led to difficulties in predicting churn with high precision. The models often struggled with false positives for the churn class.

## How to Run the Notebook
1. Clone the repository and navigate to the project directory.
2. Install the necessary dependencies using the command:
   ```
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:
   ```
   jupyter notebook "Amit Mohite - Telecom Churn Prediction.ipynb"
   ```
4. Run the cells sequentially to replicate the results and observe the model performance.

## Dependencies
- Python 3.7+
- Jupyter Notebook
- pandas, numpy, scikit-learn, xgboost, matplotlib

## Future Work
- **Improve Churn Precision**: Focus on improving the precision for the churn class to reduce false positives.
- **Model Optimization**: Experiment with ensemble techniques or neural networks for better performance.
- **Customer Segmentation**: Explore customer segmentation to understand different customer groups better and target retention strategies more effectively.

## Author
Amit Mohite

For any queries, feel free to contact me via GitHub or email (mohite.amit@gmail.com)

