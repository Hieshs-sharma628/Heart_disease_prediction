# Heart Disease Risk Prediction

**GitHub description:** A Streamlit machine-learning app that uses a trained Support Vector Machine to estimate heart disease risk from selected clinical measurements.

## Project description

This project is an interactive web application for exploring a machine-learning approach to heart disease risk prediction. Built with Streamlit, it lets a user enter a set of health measurements and observe the output of a trained Support Vector Machine (SVM) model. The form includes age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, resting electrocardiogram, maximum heart rate, exercise-induced angina, ST depression (Oldpeak), and ST slope.

When the user selects **Predict**, the application arranges the supplied values into the feature columns expected by the saved model, fills in absent one-hot encoded categories, applies the saved scaler, and requests a prediction. The result is presented as either a high-risk or low-risk indication. The repository also contains a CSV dataset and a Jupyter notebook for working with the heart disease data, alongside the serialized model, scaler, and feature-column list used by the app.

This repository is intended for educational and demonstration purposes: it shows how a trained model and preprocessing artifacts can be connected to a simple interactive interface. It is not a clinical tool. Its output is not a diagnosis or medical advice, and it should not be used to make healthcare decisions. Model quality depends on the data and training process; users should seek advice from a qualified healthcare professional about health concerns.

## Requirements

- Python
- Streamlit
- pandas
- scikit-learn
- joblib

## Run locally

1. Clone or download this repository.
2. Open a terminal in the project folder and install the dependencies:

   ```bash
   python -m pip install streamlit pandas scikit-learn joblib
   ```

3. Start the application:

   ```bash
   streamlit run app.py
   ```

The model and preprocessing files (`SVM_heart_model.pkl`, `scaler_heart.pkl`, and `columns_heart.pkl`) must remain in the project folder when you run the app.
