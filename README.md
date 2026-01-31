# 📈 Advanced Financial Prediction Dashboard

An all-in-one financial analytics platform combining powerful machine learning forecasting with real-time market insights. This application provides a sophisticated dashboard for investors and analysts to predict asset prices, optimize portfolios, and detect market anomalies.

## ✨ Features

*   **Advanced Price Forecasting**: Trend prediction using ARIMA, SARIMA, Holt-Winters, and Exponential Smoothing models.
*   **Interactive Dashboard**: Built with Streamlit for seamless user interaction and data visualization.
*   **Real-Time Anomaly Detection**: Statistical Z-score analysis to identify significant market deviations.
*   **Personalized Investment Advisor**: Tailored investment advice based on user risk tolerance and financial goals.
*   **Smart Portfolio Optimizer**: Optimize asset allocation to maximize expected returns.
*   **Multi-Market Arbitrage**: Detect price discrepancies across global markets.
*   **Technical Analysis**: Buy/Sell signals based on RSI and SMA indicators.
*   **Global Asset Coverage**: Support for Equities, Cryptos, ETFs, Indices, and Funds via Yahoo Finance.
*   **News & Sentiment**: Integrated news aggregation with NLP-based sentiment analysis.

## 🛠️ Tech Stack

*   **Frontend**: [Streamlit](https://streamlit.io/)
*   **Backend**: [Flask](https://flask.palletsprojects.com/)
*   **Machine Learning**: [Statsmodels](https://www.statsmodels.org/), [Scikit-learn](https://scikit-learn.org/)
*   **Data Processing**: [Pandas](https://pandas.pydata.org/), [NumPy](https://numpy.org/)
*   **Visualization**: [Plotly](https://plotly.com/)
*   **Data Sources**: [Yahoo Finance (yfinance)](https://pypi.org/project/yfinance/), [Pandas TA](https://github.com/twopirllc/pandas-ta)

## 🚀 Installation

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/finance-dashboard.git
    cd finance-dashboard
    ```

2.  **Create a virtual environment** (optional but recommended):
    ```bash
    python -m venv venv
    # Windows
    venv\Scripts\activate
    # macOS/Linux
    source venv/bin/activate
    ```

3.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: If `requirements.txt` is missing, install the key packages manually: `flask flask-cors streamlit pandas numpy yfinance pandas_ta plotly statsmodels scikit-learn textblob requests tenacity`)*

## 🖥️ Usage

The application requires both the Flask backend and Streamlit frontend to be running simultaneously.

1.  **Start the Backend**:
    Open a terminal and run:
    ```bash
    python backy.py
    ```
    The API will start at `http://127.0.0.1:5000`.

2.  **Start the Frontend**:
    Open a new terminal window and run:
    ```bash
    streamlit run fronty.py
    ```
    The dashboard will open in your browser at `http://localhost:8501`.

## 📂 Project Structure

*   `backy.py`: Flask backend handling API requests, model training, and data serving.
*   `fronty.py`: Streamlit frontend for the interactive user interface.
*   `FinanceDatabase/`: Local storage for financial CSV data.
*   `trained_models/`: Directory for saving trained model artifacts.
*   `static/plots/`: Generated forecast plots.
*   `improved_app.log` / `improved_frontend.log`: Application logs.

## ⚠️ Disclaimer

This application is for educational and informational purposes only. It does not constitute financial advice. Always conduct your own research before making investment decisions.

## 📄 License

[MIT License](LICENSE)
