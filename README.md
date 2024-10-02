# Nifty-50
This project focuses on predicting the stock market using two types of models: regression and classification. The dataset contains various features like `Open`, `High`, `Low`, `Previous Close`, `Last Traded Price`, `Change`, `Percentage Change`, `Volume`, `Industry`, and `Series`. 
## Libraries Used

- **numpy**: For numerical computations.
- **pandas**: For data manipulation and analysis.
- **matplotlib**: For plotting and visualizing results.
- **seaborn**: For enhanced data visualization.
- **scikit-learn**: For machine learning models, preprocessing, and evaluation metrics.
  - **Model Selection and Evaluation**:
    - `train_test_split` for splitting data
    - `GridSearchCV` for hyperparameter tuning
    - `cross_val_score` for cross-validation
    - `mean_squared_error`, `mean_absolute_error` for regression metrics
    - `accuracy_score`, `recall_score`, `precision_score`, `f1_score`, `confusion_matrix`, `ConfusionMatrixDisplay`, `classification_report` for classification metrics
  - **Models**:
    - `LinearRegression` for regression tasks
    - `LogisticRegression` for binary classification tasks
    - `SVC`, `LinearSVC` for Support Vector Classification
  - **Preprocessing**:
    - `StandardScaler`, `RobustScaler` for feature scaling
## Project Structure

- **Data Preprocessing**:
  - Cleaned the dataset.
  - Handled missing values.
  - Applied One-Hot Encoding for categorical variables such as `Industry` and Label Encoding for `Series`.
  - Used **Robust Scaler** for scaling the features.

- **Regression**:
  - Built a model to predict the `Last Traded Price` using relevant features.
  - Evaluated the model with metrics such as RMSE (Root Mean Squared Error) and MAE (Mean Absolute Error).

- **Classification**:
  - Converted `Percentage Change` into a binary target (positive or negative).
  - Applied SVM with Grid Search and **Robust Scaler** for classification of the binary target.
  - Implemented LSVM (also using **Robust Scaler**) to improve classification performance.
  - Evaluated the classification models using accuracy, precision, recall, and F1-score.

- **Random Forest**:
  - Implemented a Random Forest model for:
    - **Regression**: Predicting the `Last Traded Price`.
    - **Classification**: Predicting the `Percentage Change`.
  - Compared the results of Random Forest with the SVM, LSVM, and regression models.
