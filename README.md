# Tradent

Tradent is an AI Agent that uses machine learning trading strategy through FinBERT to analyze financial news sentiment and execute bracket orders accordingly. It uses Lumibot framework integrated with the Alpaca brokerage. 


## Disclaimer

#### This project is for educational and research purposes only. It does not constitute financial advice or a recommendation to trade real money. Always conduct your own research and consult a qualified financial professional before making any investment decisions. Discretion is advised.


## Usage Guide


### 1. Clone the Repository

Clone the repository to your local machine using:

```bash
git clone https://https://github.com/haiderameez/Tradent
```


### 2. Install Dependencies

Install all the required dependencies with:

```python
pip install -r requirements.txt
```


### 3. Environment Variables
Create a `.env` file in the root directory and add your Alpaca credentials:

```.env
API_KEY=your_alpaca_api_key

API_SECRET=your_alpaca_api_secret

BASE_URL=https://paper-api.alpaca.markets
```
> Make sure you have obtained your API keys from the https://app.alpaca.markets/.


### 4. Running the Strategy

- **Backtesting:**
  
  Run the script to start backtesting:
  
  ```python
  python main.py
  ```
  This will execute the backtest for the specified date range using Yahoo Finance data.
  
- **Live Trading (Paper):**
  Once backtesting meets your expectations, you can switch to live (paper) trading by ensuring your Alpaca credentials point to the paper trading endpoint and adjusting any necessary parameters in the strategy.

- A log folder will be created where the details of the tradings can be checked.
