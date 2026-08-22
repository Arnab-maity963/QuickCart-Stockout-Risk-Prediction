# QuickCart Stockout Risk Prediction

## 1. Project Overview

QuickCart Stockout Risk Prediction is a Machine Learning based inventory management project designed to predict the risk of a product going out of stock.

The system analyzes inventory, sales, demand, ordering, lead time, and supplier-related information to determine whether a product has a high or low stockout risk.

The trained Random Forest model is integrated with a Streamlit dashboard where users can enter inventory-related information and receive a stockout risk prediction along with its probability.

---

## 2. Problem Statement

In e-commerce and retail businesses, maintaining the right inventory level is an important challenge.

If a product goes out of stock:

- Customers may not be able to purchase the product.
- Sales opportunities may be lost.
- Customer satisfaction can decrease.
- Emergency restocking may increase operational costs.

Traditional inventory management often depends on fixed thresholds or manual monitoring.

QuickCart Stockout Risk Prediction aims to provide an automated Machine Learning based approach for identifying products that are at risk of stockout.

---

## 3. Objective

The main objectives of this project are:

1. Analyze historical inventory and sales data.
2. Identify factors related to stockout risk.
3. Prepare and preprocess the dataset for Machine Learning.
4. Train a Random Forest classification model.
5. Predict whether a product is at risk of stockout.
6. Calculate the prediction probability.
7. Provide an interactive Streamlit dashboard for prediction.

---

## 4. How the Project Works

The overall workflow of the project is:

 ## Diagram : 

Historical Inventory and Sales Data
                |
                v
        Data Preprocessing
                |
                v
       Feature Engineering
                |
                v
       Machine Learning Model
                |
                v
      Random Forest Classifier
                |
                v
       Stockout Risk Prediction
                |
                v
        Streamlit Dashboard
                |
                v
       Risk and Probability


Machine Learning Approach

The project uses a supervised Machine Learning classification approach.

Algorithm Used

Random Forest Classifier

Random Forest is used because it can handle multiple features and capture complex relationships between inventory and demand-related variables.

The model learns patterns from historical data and predicts the stockout risk for new inventory information.

6. Input Features

The Streamlit dashboard accepts inventory-related inputs such as:

Inventory Level
Units Sold
Units Ordered
Demand Forecast
Lead Time Days
Supplier Reliability

The trained model contains 231 features.

The application prepares the user input according to the feature structure expected by the trained model before making a prediction.

7. Prediction Output

The system produces two main outputs:

Stockout Risk

The model predicts the stockout class.

0 = Low Risk
1 = High Risk
Prediction Probability

The system also displays the probability associated with the predicted class.

For example:

Predicted Stockout Risk: 1
Prediction Probability: 55.50%

This indicates that the model predicts a stockout risk for the given input with a probability of approximately 55.50%.

8. Streamlit Dashboard

The Streamlit dashboard provides a simple interface for interacting with the Machine Learning model.

The dashboard contains:

Project title and description
Model information
Model feature information
Inventory input fields
Prediction button
Stockout risk result
Prediction probability

The dashboard allows users to interact with the trained model without directly working with Python code.

9. Technologies Used
Programming Language
Python
Machine Learning
Scikit-learn
Random Forest Classifier
Data Processing
Pandas
NumPy
Model Serialization
Joblib
Dashboard
Streamlit
Development Environment
Jupyter Notebook
Anaconda
VS Code or any Python-compatible editor
Version Control
Git
GitHub
10. Project Structure
QuickCart_Stockout_Risk/
|
├── app.py
├── quickcart_stockout_model.pkl
├── quickcart_model_features.pkl
├── quickcart_target_encoder.pkl
├── model_training.ipynb
├── dataset.csv
├── requirements.txt
└── README.md

Note: File names may vary depending on the final project implementation.

11. Installation

Clone the repository:

Move into the project directory:

cd QuickCart-Stockout-Risk

Create and activate a virtual environment if required:

python -m venv venv

Windows:

venv\Scripts\activate

Install the required dependencies:

pip install -r requirements.txt

12. Running the Application

Run the Streamlit application using:

streamlit run app.py

After running the command, Streamlit will provide a local URL similar to:


13. Using the Dashboard

Follow these steps:

Open the Streamlit dashboard.
Enter the inventory information.
Enter the sales and demand-related values.
Enter the lead time and supplier reliability.
Click the "Predict Stockout Risk" button.
The system sends the input to the trained Random Forest model.
The dashboard displays the predicted stockout risk.
The dashboard also displays the prediction probability.
14. Example Workflow

Example input:

Inventory Level: 100
Units Sold: 20
Units Ordered: 30
Demand Forecast: 25
Lead Time Days: 5
Supplier Reliability: 0.8

The application processes the input and sends it to the trained Machine Learning model.

Example output:

Predicted Stockout Risk: 1
Prediction Probability: 55.50%

The result indicates that the model has identified the given inventory situation as a stockout-risk case.

15. Benefits

The project can help businesses:

Identify potential stockout situations.
Monitor inventory risk.
Support inventory planning.
Reduce the possibility of unexpected stockouts.
Make data-driven inventory decisions.
Provide an easy interface for Machine Learning predictions.

16. Limitations

The prediction quality depends on the quality and representativeness of the training dataset.

The model may not accurately predict situations that are significantly different from the historical data used for training.

The current system is a prediction prototype and does not automatically place inventory orders.

17. Future Enhancements

Possible future improvements include:

Real-time inventory data integration.
Automatic database connectivity.
Product-wise stockout monitoring.
Inventory alerts and notifications.
Demand forecasting.
Automatic reorder recommendations.
Advanced Machine Learning models.
Interactive analytics and visualization.
Cloud deployment.
Integration with e-commerce inventory systems.
18. Project Outcome

The project successfully demonstrates an end-to-end Machine Learning workflow for inventory stockout risk prediction.

The workflow starts with historical data, performs data preprocessing and feature preparation, trains a Random Forest classification model, saves the trained model, and integrates it with a Streamlit dashboard.

The final application allows users to provide inventory-related information and receive a stockout risk prediction and probability.

19.  ## Conclusion : 

QuickCart Stockout Risk Prediction demonstrates how Machine Learning can be applied to inventory management.

By predicting potential stockout risks before they occur, the system can support better inventory planning and help businesses take preventive actions.

The combination of Python, Scikit-learn, Random Forest, Joblib, and Streamlit provides a complete workflow from Machine Learning model development to an interactive prediction application.

20. Author

Developed as a Machine Learning and Data Science project.

Project: QuickCart Stockout Risk Prediction

Domain: Machine Learning, Data Science, Inventory Management
