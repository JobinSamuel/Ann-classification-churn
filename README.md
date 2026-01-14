# Customer Churn Prediction (ANN + Streamlit)

This project predicts whether a bank customer is likely to **churn (exit the bank)** using an **Artificial Neural Network (ANN)** built with **TensorFlow/Keras**.
The trained model is deployed using a simple **Streamlit web application** for real-time predictions.

---

## What I Did in This Project 

* Loaded and explored the **Churn_Modelling.csv** dataset
* Dropped irrelevant columns (RowNumber, CustomerId, Surname)
* Performed encoding:

  * **LabelEncoder** for Gender
  * **OneHotEncoder** for Geography
* Scaled numerical features using **StandardScaler**
* Trained an ANN model using **TensorFlow/Keras**
* Used **EarlyStopping** to reduce overfitting
* Logged training runs using **TensorBoard**
* Saved all preprocessing + model artifacts:

  * label_encoder_gender.pkl
  * onehot_geo.pkl
  * scaler.pkl
  * model.keras
* Built a Streamlit UI to enter customer details and predict churn

---

## Model Inputs

* CreditScore
* Geography
* Gender
* Age
* Tenure
* Balance
* NumOfProducts
* HasCrCard
* IsActiveMember
* EstimatedSalary

---

## Output

* The app returns a **churn probability**
> 0.5 - customer likely to churn
<= 0.5 - customer not likely to churn



