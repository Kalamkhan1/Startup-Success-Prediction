# Startup Success Prediction: README

## Project Overview

This project aims to predict the success of startups using machine learning techniques. The dataset used contains various features such as funding rounds, geographical information, funding amounts, and categorical attributes representing the type and state of the startups. Multiple machine learning models were implemented and evaluated to identify the most effective approach for classification.

---

## Dataset Details

The dataset was sourced from an online repository and contains 48 columns, including:

- **Numerical Features**: funding rounds, total funding, average participants, milestones, etc.
- **Categorical Features**: category codes, state codes, and status labels (target variable).
- **Target Variable**: `status` (represents the startup's success or failure).

### Dataset URL

The dataset can be accessed [here](https://raw.githubusercontent.com/dphi-official/Datasets/master/startupdata/training_set_label.csv).

### Preprocessing Steps

1. Dropped irrelevant columns.
2. Handled missing values using pipelines:
   - **Numerical Features**: Filled with constant values and normalized using `MinMaxScaler`.
   - **Categorical Features**: Filled missing values with "NA" and encoded using `OneHotEncoder`.
3. Encoded the target variable using `LabelEncoder`.

---

## Exploratory Data Analysis (EDA)

1. **Target Variable Distribution**: Visualized the counts of each class in the `status` column.
2. **Correlation Analysis**: Displayed a heatmap of correlations between features and the target variable.
3. **Feature Distributions**: Examined numerical features and their distributions across different startup statuses using boxplots.
4. **Categorical Feature Analysis**: Visualized the distribution of categories and their correlation with the target.

---

## Models Implemented

1. **Random Forest Classifier**:

   - Accuracy: 79.32%
   - Precision: 78.41%
   - Recall: 74.82%
   - F1-Score: 75.97%

2. **XGBoost Classifier**:

   - Accuracy: 75.00%
   - Precision: 72.58%
   - Recall: 72.49%
   - F1-Score: 72.53%

3. **LightGBM Classifier**:

   - Accuracy: 76.8%
   - Precision: 74.4%
   - Recall: 74.9%
   - F1-Score: 74.7%

4. **CatBoost Classifier**:

   - Accuracy: 78.39%
   - Precision: 76.31%
   - Recall: 76.31%
   - F1-Score: 76.31%

### Evaluation Metrics

- **Accuracy**: Proportion of correctly classified samples.
- **Precision**: Ratio of true positives to all predicted positives.
- **Recall**: Ratio of true positives to all actual positives.
- **F1-Score**: Harmonic mean of precision and recall.

---

## Libraries Used

- `pandas`, `numpy`: Data manipulation and processing.
- `matplotlib`, `seaborn`: Visualization.
- `scikit-learn`: Machine learning pipelines and model implementation.
- `xgboost`, `lightgbm`, `catboost`: Advanced gradient boosting models.

---

## Future Improvements

1. Implement hyperparameter tuning for better model performance.
2. Include more advanced feature engineering techniques.
3. Explore ensemble methods for further accuracy improvements.

---

## Contributors

- **Mohammed Abdul Kalam Khan**

---

## License

This project is licensed under the MIT License.

