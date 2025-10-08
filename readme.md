# Fraud Detection Prediction App

This project is a **Machine Learning + Streamlit web application** that predicts whether a transaction is **fraudulent or not** based on the transaction details provided by the user.

---

## Simple Flow Explanation

1. **User Input:**
   - The user fills in transaction details in the Streamlit app.  
     *(Transaction Type, Amount, Old Balance, New Balance, etc.)*

2. **Data Preparation:**
   - The app creates a **mini dataset (DataFrame)** from the user's input.

3. **Model Processing:**
   - The trained Machine Learning model applies its learned rules on the input data, such as:
     - Whether the balance difference is abnormal  
     - Whether the transaction type looks suspicious  

4. **Prediction:**
   - The model outputs:
     - `1` → Fraudulent Transaction  
     - `0` → Legitimate Transaction  

5. **Result Display:**
   - The Streamlit app displays the result on the screen:
     - **Fraud Alert!** if the transaction seems risky  
     - **Transaction Safe** if it appears normal  

---

## How the Model Works

- The model is trained using historical transaction data.
- It learns the relationship between various features like transaction type, amount, and balance differences.
- Once trained, it can predict the probability of a new transaction being fraudulent.

---

## Usage

1. Open the Streamlit app interface.
2. Enter the required transaction details:
   - Transaction Type  
   - Amount  
   - Old Balance (Sender)  
   - New Balance (Sender)  
   - Old Balance (Receiver)  
   - New Balance (Receiver)
3. Click the **"Predict"** button.
4. The app will display whether the transaction is **Fraudulent** or **Not Fraudulent**.

---

## How to Run the App

1. Clone or download this repository.  
   ```bash
   git clone https://github.com/yourusername/fraud-detection-app.git
   cd fraud-detection-app
