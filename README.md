# Home Credit Default Risk Portfolio
### Author: Zac Mendenhall

## Project Overview
This project predicts the likelihood of loan default using the Home Credit Default dataset from Kaggle. 
Included here is solely my individual code I contributed to the project, not the whole project itself or our convlusions.

## My Contributions
- Cleaned and preprocessed the data, including missing value imputation, feature transformations, and encoding.
- Addressed class imbalance using techniques like class weighting and SMOTE.
- Built and evaluated Random Forest models, tuning hyperparameters to optimize performance.

## Key Findings
- Class imbalance significantly impacted the model’s ability to identify defaults (minority class).
- SMOTE and class weighting slightly improved recall and AUC but still required further optimization.
- Feature importance analysis identified critical predictors, such as `AMT_CREDIT` and `DAYS_BIRTH`.

## Notebooks
- **Data Preprocessing and EDA**: `data_cleaning.Rmd`
- **Random Forest Modeling**: `random_forest_modeling.Rmd`
- **Class Imbalance Strategies (Weighted and SMOTE)**: `class_imbalance_solutions.Rmd`

## Business Value
This project supports financial institutions in:
- Identifying high-risk borrowers.
- Enhancing loan approval processes.
- Minimizing financial losses through accurately predicting those who default and those who won't

## Results
| Metric        | Basic RF | Weighted RF | RF with SMOTE |
|---------------|----------|-------------|---------------|
| Accuracy      | 91%      | 91%         | 91.7%         |
| Recall (Class 1) | 0.0037   | 0.0060      | 0.006         |
| AUC           | 0.71     | 0.70        | 0.68          |

## Next Steps
- Explore additional resampling techniques to address class imbalance.
- Apply model interpretability tools like SHAP or LIME to explain predictions.
- Full project can be provided at request to myself to see full results and work (our XGBoost model performed best and the Random Forest model was the worst performing model)

## Challenges Faced
- Class imbalance made it difficult for the models to identify minority class samples well
- Computer memory limitations meant we had to adapt and make changes to models due to large processing times
- In my case I preferred R over Python but my group worked in Python so I had to adapt

## What I Learned
- Learned how to better handle imbalanced datasets
- Learned to recognize when a model was useful or not compared to others (Random Forest wasn't the best in this case)
- Learned how to work in a team that didn't meet physically and how to work in code amongst said team

## Repository Structure
- `data_cleaning.Rmd`: Preprocessing and feature engineering.
- `random_forest_modeling.Rmd`: Model building and evaluation.
- `plots/`: Visualizations of feature importance and ROC curves.
- `README.md`: Project overview and results.

## Contact
- LinkedIn: [[Your LinkedIn Profile](https://www.linkedin.com/in/zachary-mendenhall/)]
