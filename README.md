# Credit Wise

Credit Wise is a machine learning notebook for predicting loan approval decisions from applicant, credit, income, loan, and property information.

The notebook includes the full workflow with saved outputs:

- Data loading from `loan_approval_data.csv`
- Missing value handling with `SimpleImputer`
- Exploratory data analysis and visualizations
- Categorical feature encoding
- Correlation analysis
- Train-test split and feature scaling
- Model training and evaluation
- Feature engineering experiments

## Project Files

| File | Description |
| --- | --- |
| `credit_wise.ipynb` | Executed Jupyter notebook with code, plots, and output cells saved. |
| `loan_approval_data.csv` | Dataset used by the notebook. |
| `requirements.txt` | Python packages needed to run the notebook. |

## Models Evaluated

The notebook evaluates:

- Logistic Regression
- K-Nearest Neighbors
- Naive Bayes

Saved notebook results show Naive Bayes as the best model by precision in the initial model comparison.

After feature engineering, the saved metrics include:

| Model | Precision | Recall | Accuracy | F1 Score |
| --- | ---: | ---: | ---: | ---: |
| Logistic Regression | 0.8333 | 0.7477 | 0.8697 | 0.7882 |
| KNN | 0.6883 | 0.4953 | 0.7636 | 0.5761 |
| Naive Bayes | 0.8523 | 0.7009 | 0.8636 | 0.7692 |

## How to Run

1. Clone the repository.
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook:

   ```bash
   jupyter notebook credit_wise.ipynb
   ```

4. Run the cells from top to bottom.

## Dataset Columns

The dataset contains 1,000 rows and includes fields such as:

- Applicant income and coapplicant income
- Employment status
- Age and marital status
- Dependents
- Credit score
- Existing loans
- Debt-to-income ratio
- Savings and collateral value
- Loan amount, loan term, and loan purpose
- Property area
- Education level
- Gender
- Employer category
- Loan approval status

## Tech Stack

- Python
- Jupyter Notebook
- pandas
- NumPy
- seaborn
- Matplotlib
- scikit-learn
