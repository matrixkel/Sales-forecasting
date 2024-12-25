# Sales Forecasting Model

This project is a machine learning application to predict car purchase amounts based on various customer attributes. It utilizes Python and popular data science libraries to build and evaluate a predictive model.

## Objective
The goal of this project is to forecast sales (car purchase amount) using customer data, enabling businesses to optimize their marketing strategies and maximize revenue.

## Features Used
The dataset includes the following features:
- **country**: The country of the customer.
- **gender**: Gender encoded as 0 or 1.
- **age**: Customer's age.
- **annual Salary**: Customer's annual income.
- **credit card debt**: Debt accumulated on the credit card.
- **net worth**: Customer's net worth.

The target variable is **car purchase amount**, which indicates the spending on car purchases.

## Steps in the Project

1. **Data Loading and Preprocessing**
    - Unnecessary columns like `customer name` and `customer e-mail` are dropped.
    - Categorical variables (e.g., `country`) are encoded using one-hot encoding.
    - Numerical variables are standardized using `StandardScaler`.

2. **Model Selection and Pipeline**
    - A `RandomForestRegressor` is chosen for regression tasks.
    - A preprocessing pipeline handles scaling and encoding, ensuring seamless data transformation.

3. **Training and Evaluation**
    - Data is split into training (80%) and test (20%) sets.
    - The model is trained on the training set and evaluated on the test set using:
        - **Mean Squared Error (MSE)**: Measures the average squared difference between actual and predicted values.
        - **R-squared (R²)**: Indicates the proportion of variance explained by the model.
        - **Accuracy**: Calculates how often the model's predictions align with the trend of actual values.

4. **Model Saving**
    - The trained model is saved to Google Drive for future use.

## Key Results
After training and testing, the model outputs the following evaluation metrics:
- **Mean Squared Error (MSE):** Quantifies prediction errors.
- **R² Score:** Measures how well the model fits the data.
- **Accuracy:** Measures prediction alignment with actual trends.

## Prerequisites
To run this project, you need:
- Python (3.6 or higher).
- Libraries: `pandas`, `numpy`, `scikit-learn`, `joblib`, and `os`.
- Access to Google Colab (for saving the model to Google Drive).

## How to Run
1. **Upload the Dataset**
   - Place your dataset (e.g., `car_purchasing.csv`) in the appropriate directory.
2. **Run the Code**
   - Execute the Python script step-by-step in a Colab environment.
3. **Mount Google Drive**
   - Ensure your Google Drive is mounted to save the trained model.
4. **Check Results**
   - Metrics such as MSE, R², and accuracy will be printed for evaluation.
5. **Retrieve the Model**
   - The trained model is saved in `My Drive` under the name `sales_forecast_model.pkl`.

## Future Enhancements
- Experiment with different models like Gradient Boosting or Neural Networks.
- Incorporate additional features to improve prediction accuracy.
- Develop a web interface for real-time predictions.

## License
This project is open-source and available under the MIT License.

---
For any questions or contributions, feel free to reach out!

