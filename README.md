# Customer Churn Analysis

## Project Overview

This project performs a comprehensive analysis of customer churn in a telecommunications company. The analysis includes exploratory data analysis (EDA) to understand customer patterns and predictive modeling to identify customers likely to churn.

## Objective

The goal is to:
- Analyze customer data to identify patterns and characteristics of customers who churn
- Build predictive models to identify customers at risk of leaving
- Provide insights to help reduce customer churn rates

## Project Structure

The project consists of the following components:

### 1. **Churn Analysis - EDA.ipynb**
   - Exploratory Data Analysis of the Telco customer churn dataset
   - Data loading and preprocessing
   - Statistical analysis and visualization
   - Feature exploration and distribution analysis
   - Identification of key patterns and correlations

### 2. **Churn Analysis - Model Building.ipynb**
   - Predictive modeling for customer churn prediction
   - Data preparation and feature engineering
   - Train-test split
   - Decision Tree Classifier implementation
   - Model evaluation and performance metrics
   - Handling class imbalance using SMOTEENN

### 3. **Data Files**
   - `WA_Fn-UseC_-Telco-Customer-Churn.csv`: Original telco customer dataset
   - `tel_churn.csv`: Processed dataset used for model building
   - `Customer_churn_database.csv`: Additional customer data reference

## Technologies & Libraries

- **Python 3.x**
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: scikit-learn
- **Imbalanced Data Handling**: imbalanced-learn (SMOTEENN)

## Key Dependencies

```
pandas
numpy
seaborn
matplotlib
scikit-learn
imbalanced-learn
```

## Dataset Information

The dataset contains:
- **Customer Demographics**: Age, gender, senior citizen status
- **Account Information**: Contract type, tenure, monthly charges, total charges
- **Services**: Internet service, phone service, streaming services, etc.
- **Target Variable**: Churn (Yes/No)

### Sample Size
- Multiple thousands of customer records
- Historical churn information for model training

## Methodology

### EDA Phase
1. Data loading and inspection
2. Descriptive statistics
3. Data type validation
4. Distribution analysis
5. Correlation analysis
6. Categorical variable exploration
7. Visual insights through charts and plots

### Model Building Phase
1. Feature preparation (dropping unnecessary columns)
2. Feature and target separation
3. Data splitting (80/20 train-test split)
4. Decision Tree Classifier configuration
5. Model training
6. Prediction and evaluation
7. Performance metrics analysis

### Model Specifications
- **Algorithm**: Decision Tree Classifier
- **Criterion**: Gini impurity
- **Max Depth**: 6
- **Min Samples Leaf**: 8
- **Class Imbalance Handling**: SMOTEENN (Synthetic Minority Oversampling with Edited Nearest Neighbors)

## Key Metrics & Evaluation

The models are evaluated using:
- **Confusion Matrix**: TP, TN, FP, FN
- **Recall Score**: Emphasis on identifying actual churners
- **Classification Report**: Precision, recall, F1-score
- **Accuracy**: Overall model performance

## How to Use

1. **Install Dependencies**:
   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn imbalanced-learn
   ```

2. **Open the Notebooks**:
   - Start with `Churn Analysis - EDA.ipynb` to explore the data
   - Proceed to `Churn Analysis - Model Building.ipynb` for model development

3. **Run the Cells**:
   - Execute cells sequentially to load data, perform analysis, and build models
   - Review visualizations and statistics to gain insights

4. **Interpret Results**:
   - Analyze the EDA findings to understand churn drivers
   - Review model performance metrics
   - Use predictions to identify at-risk customers

## Key Insights (Expected)

- Identification of demographic segments with higher churn rates
- Impact of contract types and service subscriptions on churn
- Customer tenure patterns and their relationship to churn
- Price sensitivity and monthly charge influence on retention

## Model Performance

The Decision Tree model provides:
- Quick and interpretable predictions
- Feature importance rankings
- Clear decision boundaries for churn prediction
- Balanced approach to handling class imbalance through SMOTEENN

## Future Enhancements

- Implement additional classification algorithms (Random Forest, Gradient Boosting, SVM)
- Perform hyperparameter tuning for better performance
- Ensemble methods combining multiple models
- Real-time prediction pipeline development
- Customer segmentation analysis
- Recommendation engine for retention strategies
