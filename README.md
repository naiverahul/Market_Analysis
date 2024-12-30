# Bank Marketing Data Analysis and Modeling

This repository contains a Jupyter Notebook for performing data analysis and modeling on the Bank Marketing dataset from the UCI Machine Learning Repository. The objective is to predict whether a client will subscribe to a term deposit based on various features.

## Project Workflow

### 1. Import Libraries and Fetch Dataset
- Import libraries for data manipulation, visualization, and modeling.
- Fetch the Bank Marketing dataset using `fetch_ucirepo`.

### 2. Data Preparation
- Combine features and target variables into a single DataFrame.
- Rename columns for clarity.
- Remove columns with missing or irrelevant data.
- Display initial rows and check for missing values.

### 3. Exploratory Data Analysis (EDA)
- Provide summary statistics of the dataset.
- Visualize the distribution of the target variable.
- Plot histograms for numerical features.
- Analyze categorical features using boxplots.

### 4. Data Encoding
- Apply Label Encoding to categorical features.
- Combine encoded categorical and numerical features.
- Display the correlation matrix and target correlations.

### 5. Data Splitting
- Split the dataset into training and testing sets.
- Apply SMOTE to balance the training set for the target variable.

### 6. Data Scaling
- Identify numerical and categorical features.
- Scale features using `StandardScaler`.
- Summarize statistics of scaled training and testing sets.

### 7. Baseline Model - Logistic Regression
- Build and cross-validate a baseline logistic regression model.
- Summarize cross-validation results.

### 8. Complex Model - Random Forest
- Perform hyperparameter tuning on a Random Forest model using `RandomizedSearchCV`.
- Identify optimal parameters and evaluate cross-validation performance.

### 9. Model Evaluation
- Assess the best Random Forest model on the test set.
- Compare performance with the baseline logistic regression model.
- Provide classification reports for both models.

## Libraries Used
- `pandas`, `numpy` for data manipulation
- `matplotlib`, `seaborn` for data visualization
- `scikit-learn` for machine learning models and preprocessing
- `imblearn` for handling imbalanced datasets
- `IPython`, `tabulate`, `ucimlrepo` for utilities and dataset fetching

## Dataset Details
- **Name:** Bank Marketing Dataset  
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)  
- **Dataset ID:** 222  
- **Objective:** Predict client subscription to a term deposit (`yes` or `no`).

## How to Use
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/bank-marketing-analysis.git
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Open the Jupyter Notebook and follow the workflow:
    ```bash
    jupyter notebook
    ```

## Results and Insights
The notebook demonstrates data preparation, exploratory analysis, and modeling techniques to predict client behavior. It compares the performance of a baseline Logistic Regression model with a tuned Random Forest model, highlighting the improvements achieved with advanced modeling techniques.

## Contributions
Contributions are welcome! If you have suggestions or improvements, feel free to submit a pull request.


