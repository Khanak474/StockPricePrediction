# 📈 Neural Network-Based Stock Price Prediction

## 📌 Overview
This project focuses on **stock price prediction using deep learning models**, specifically:

- Long Short-Term Memory (**LSTM**)  
- Gated Recurrent Unit (**GRU**)  
- Bidirectional LSTM (**BiLSTM**)  

The goal is to compare these models and identify the most effective architecture for **time-series forecasting and stock movement prediction**.

---

## 🎯 Objectives
- Predict future stock prices using historical data  
- Classify stock movement direction (**Up / Down**)  
- Compare performance of LSTM, GRU, and BiLSTM  
- Evaluate models using regression and classification metrics  

---

## 📊 Dataset
- Source: **Yahoo Finance (via yfinance API)**  
- Features used:
  - Open price  
  - Close price  

### 🔧 Preprocessing
- Normalization using MinMaxScaler  
- Sequence creation using **60-day sliding window**  
- Train-Test split: 80:20  

---

## 🧠 Models Used

### 🔹 LSTM
- Captures long-term dependencies  
- Uses input, forget, and output gates  

### 🔹 GRU
- Faster and more efficient than LSTM  
- Uses update and reset gates  

### 🔹 BiLSTM
- Processes data in both forward & backward directions  
- Captures richer temporal patterns  
- Achieved best performance in this project  

---

## ⚙️ Training Details
- Epochs: 50  
- Batch Size: 32  
- Optimizer: Adam  
- Loss Function: Mean Squared Error (MSE)  

---

## 📈 Evaluation Metrics

### Regression:
- MAE (Mean Absolute Error)  
- MSE (Mean Squared Error)  
- RMSE (Root Mean Squared Error)  
- Pearson Correlation  

### Classification:
- Accuracy  
- Precision  
- Recall  
- F1-Score  

---

## 📊 Results

### 🏆 Best Model: BiLSTM
- Highest correlation with actual prices  
- Lowest MAE, MSE, RMSE  
- Best classification accuracy (~57%)  

### 📌 Observations:
- LSTM → weakest performance (poor trend adaptation)  
- GRU → balanced performance (fast + accurate)  
- BiLSTM → most accurate & stable predictions  

📌 As shown in evaluation (page 15), BiLSTM consistently outperformed other models across all metrics.

---

## 📉 Visualization Insights
- BiLSTM closely tracks actual stock trends  
- GRU adapts better than LSTM  
- LSTM struggles with sudden market changes  

📌 Loss graphs (pages 19–20) show:
- BiLSTM → fastest and most stable convergence  
- GRU → good convergence  
- LSTM → slower learning  

---

## 🚀 Features
- Real-time stock data fetching  
- Future price prediction  
- Direction classification (Up/Down)  
- Comparative analysis of multiple models  

---

## 🛠️ Tech Stack
- Python  
- TensorFlow / Keras  
- NumPy, Pandas  
- Matplotlib  
- yfinance  

---

## 🔮 Future Work
- Add technical indicators (RSI, Moving Averages)  
- Integrate news sentiment analysis  
- Multi-step forecasting  
- Hybrid models (CNN + LSTM)  
- Real-time deployment  

---

## 📌 Conclusion
BiLSTM proved to be the most effective model due to its ability to capture both past and future context, making it highly suitable for **financial time-series prediction**.

---

## 👩‍💻 Author
**Khanak Gupta**  

---

## 📚 References
- Research papers on LSTM, GRU, BiLSTM  
- Financial time-series forecasting studies  
- Yahoo Finance API  

---
