# SQCC-Task
This task focuses on predicting the stock market using two types of models: regression and classification. The dataset contains various features like `Open`, `High`, `Low`, `Previous Close`, `Last Traded Price`, `Change`, `Percentage Change`, `Volume`, `Industry`, and `Series`. The is to apply machine learning techniques to predict the `Last Traded Price` and classify the `Percentage Change` as positive or negative.

## Project Structure

- **Data Preprocessing**:
  - Cleaned the dataset.
  - Handled missing values.
  - Applied One-Hot Encoding for categorical variables such as `Industry` and `Series`.
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
