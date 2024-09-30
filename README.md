# Salary Estimation App
This project is focused on predicting estimated salaries using machine learning models. The project includes a web app built using Streamlit, where users can input features like geography, gender, age, credit score, and other relevant factors to predict their estimated salary.

## Project Overview
The project leverages a pre-trained neural network model to estimate salaries based on various user inputs such as geography, gender, age, credit score, balance, and other banking-related features. The model is deployed using Streamlit for ease of use in a web-based interface.

## Installation
Install the required dependencies:
```bash
  pip install -r requirements.txt
```
Run the Streamlit app
```bash
  streamlit run streamlit_regression.py
```
## Usage

1. Open the web app. [Salary Prediction App](https://ann-salary-prediction-project-8nsrg4sxejdteo8bwezqgu.streamlit.app/)

2. Select the appropriate values for:

- Geography
- Gender
- Age
- Balance
- Credit Score
- Exited (Customer churn status)
- Tenure (Years with the bank)
- Number of Products (1 to 4)
- Has Credit Card (0 or 1)
- Is Active Member (0 or 1)
- Click Predict to get the estimated salary.

## Files Description
- `streamlit_regression.py`: The script to run the Streamlit app for salary estimation. It handles user inputs, preprocessing, and model prediction​(streamlit_regression).
- `regression_model.keras`: The pre-trained neural network model used for salary prediction.
- `onehotencoder_geography.pkl`: Pickle file containing the one-hot encoder for the Geography feature.
- `label_encoder_gender.pkl`: Pickle file containing the label encoder for the Gender feature.
- `scaler.pkl`: Pickle file containing the StandardScaler used for scaling numerical features.

The model was built using TensorFlow and the `regression_model.keras` file stores the saved model, which is loaded during app runtime for predictions.

## Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue if you find any bugs or want to improve the app.
