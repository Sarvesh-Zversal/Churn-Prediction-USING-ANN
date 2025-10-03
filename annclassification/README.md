# Customer Churn Prediction

This project predicts customer churn using an Artificial Neural Network (ANN) trained on the "Churn_Modelling.csv" dataset. It provides an interactive Streamlit web app for making predictions and includes Jupyter notebooks for experimentation and model development.

---

##  Features

- **Interactive Web App:** Enter customer details and get churn probability instantly.
- **Consistent Preprocessing:** Uses saved encoders and scaler for reliable input transformation.
- **Trained Model:** Utilizes a Keras ANN model (`model.h5`) for predictions.
- **Experimentation:** Jupyter notebooks for data exploration, feature engineering, and model training.

---

##  Project Structure

```
.
├── app.py                     # Streamlit web app
├── Churn_Modelling.csv        # Dataset
├── experiments.ipynb          # Model development and experiments
├── prediction.ipynb           # Example prediction workflow
├── model.h5                   # Trained ANN model
├── label_encoder_gender.pkl   # Saved LabelEncoder for Gender
├── onehot_encoder_geo.pkl     # Saved OneHotEncoder for Geography
├── scaler.pkl                 # Saved StandardScaler
├── logs/                      # TensorBoard logs
└── README.md                  # Project documentation
```

---

##  How to Run

### 1. Install Requirements

It is recommended to use a virtual environment.

create and activate a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

```sh
pip install -r requirements.txt
```

If you don't have a `requirements.txt`, install dependencies manually:

```sh
pip install streamlit tensorflow scikit-learn pandas numpy
```

### 2. Run the Streamlit App

```sh
streamlit run app.py
```

### 3. Use the App

- Open the provided local URL in your browser.
- Enter customer details (Geography, Gender, Age, etc.).
- View the predicted churn probability and outcome.

---

##  Model Inputs

- **CreditScore**
- **Geography** (France, Germany, Spain)
- **Gender** (Male, Female)
- **Age**
- **Tenure**
- **Balance**
- **NumOfProducts**
- **HasCrCard** (0 or 1)
- **IsActiveMember** (0 or 1)
- **EstimatedSalary**

---

##  Files

- `app.py`: Main Streamlit app.
- `experiments.ipynb`: Data exploration, preprocessing, and model training.
- `prediction.ipynb`: Example prediction pipeline.
- `model.h5`: Trained Keras model.
- `label_encoder_gender.pkl`: LabelEncoder for Gender.
- `onehot_encoder_geo.pkl`: OneHotEncoder for Geography.
- `scaler.pkl`: StandardScaler for input features.

---

##  Notes

- Ensure all `.pkl` and `.h5` files are present in the project directory.
- The model and encoders were trained and saved in the Jupyter notebooks.
- For best results, use the same preprocessing steps as in the training pipeline.

---

##  License

This project is for educational purposes.