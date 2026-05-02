# SyriaTel Customer Churn Analysis

## Overview
This project builds a classification model to predict customer churn for SyriaTel, a telecommunications company. The goal is to help SyriaTel reduce revenue loss by identifying customers who are likely to stop doing business with them.

## Business and Data Understanding
### Stakeholder Audience
The primary audience is SyriaTel's business and retention team. They are interested in reducing revenue lost due to customers who don't stick around. By predicting churn early, the retention team can intervene with targeted offers and support.

### Dataset
The dataset contains 3,333 customer records with 21 features including call usage, charges, account information, and customer service calls. The target variable is churn — whether a customer left SyriaTel or not. Only 14.5% of customers churned, making this an imbalanced classification problem.

## Modeling
Three models were built iteratively:
1. *Logistic Regression* — simple baseline model
2. *Decision Tree* — improved churn recall significantly
3. *Tuned Decision Tree* — final model with optimized hyperparameters (max_depth=5, min_samples_split=10)

## Evaluation
The Tuned Decision Tree is the final recommended model:
- *94% accuracy* on test data
- *88% precision* for identifying churners
- *66% recall* for catching churners
- Minimal overfitting — training (95%) and test (94%) performance are very close

## Conclusion
By deploying this model, SyriaTel can proactively identify at-risk customers and take action before they leave, significantly reducing revenue loss. Next steps include trying Random Forest and addressing class imbalance with SMOTE.

## Repository Structure
├── README.md
├── project.ipynb
├── bigml_59c28831336c6604c800002a.csv