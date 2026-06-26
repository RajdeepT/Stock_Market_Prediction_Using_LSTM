# 📈 Stock Market Prediction using LSTM and Technical Indicators

A deep learning-based stock market prediction system that uses **Long Short-Term Memory (LSTM)** networks along with technical indicators such as **Exponential Moving Average (EMA)** and **Parabolic SAR (PSAR)** to predict the future direction of stock prices.

---

## 🚀 Features

- Download historical stock data using Yahoo Finance
- Automatic data preprocessing and cleaning
- Technical indicator calculation
  - Exponential Moving Average (EMA)
  - Parabolic SAR (PSAR)
  - Daily Returns
  - Trend Feature
- Data visualization
  - Volume chart
  - Trend plot
  - Daily return plot
  - Correlation heatmap
- Multi-feature LSTM model
- Early stopping to reduce overfitting
- Predict future stock movement
- Performance evaluation using R² Score

---

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Yahoo Finance API (yfinance)

---

## 📂 Project Structure

```
README.md
Stock_Market_Prediction_LSTM_model
```

---

## 📊 Features Used for Prediction

The model uses the following features:

- Trend
- Volume
- EMA (60-day)
- Parabolic SAR (PSAR)
- Daily Return

Target Variable:

- Direction
  - 1 → Bullish
  - 0 → Bearish

---

## 🧠 Model Architecture

```
Input Sequence
      │
      ▼
LSTM (50 Units)
      │
Dropout (0.2)
      │
LSTM (30 Units)
      │
Dropout (0.2)
      │
Dense (Sigmoid)
      │
Prediction
```

---

## 📈 Workflow

1. Download historical stock data.
2. Calculate technical indicators.
3. Generate prediction features.
4. Scale data using StandardScaler.
5. Create sequential time-series data.
6. Train the LSTM model.
7. Predict future stock movement.
8. Evaluate model performance.

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/RajdeepT/Stock_Market_Prediction_Using_LSTM.git
cd Stock_Market_Prediction_Using_LSTM
```

Install dependencies

```bash
pip install pandas numpy matplotlib seaborn tensorflow scikit-learn yfinance
```

---

## ▶️ Usage

Run the notebook or execute the Python script.

The program will ask:

```
Enter the number of months you want to predict:
```

After training, the model predicts future stock movement and displays the evaluation score.

---

## 📉 Visualizations

The project generates:

- Volume over time
- Trend over time
- Daily Return plot
- Correlation Heatmap

---

## 📌 Example Stock

Current implementation uses:

```
INFY.NS
```

This can easily be changed to any stock supported by Yahoo Finance.

Examples:

- AAPL
- MSFT
- TSLA
- TCS.NS
- RELIANCE.NS

---

## 🔮 Future Improvements

- Add more technical indicators (RSI, MACD, Bollinger Bands)
- Hyperparameter tuning
- GRU and Transformer models
- Multi-stock prediction
- Streamlit web application
- Sentiment analysis integration
- Model deployment using Flask or FastAPI

---

## 📄 License

This project is intended for educational and research purposes.

---

## 👤 Author

**Rajdeep Thakur**

B.Tech in Information Technology  
Machine Learning & Data Analytics Enthusiast

---

### ⭐ If you found this project useful, consider giving it a star!
