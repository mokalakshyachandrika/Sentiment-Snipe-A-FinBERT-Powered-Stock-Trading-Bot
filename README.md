# 📈 Sentiment Snipe: Stock Trading Bot using FinBERT and LumiBot

A real-time stock trading bot that uses **FinBERT** to analyze market sentiment from news headlines and places trades on **Alpaca**. Optionally, it integrates with **LumiBot** to demonstrate strategy automation.

---

## 📌 Overview

This project performs:

- 📥 Fetching stock market news (via Alpaca API)
- 🔍 Sentiment analysis using FinBERT (positive / negative / neutral)
- 💹 Placing BUY/SELL orders based on sentiment confidence
- 🤖 Optional LumiBot strategy setup for backtesting/live execution
- 📈 Display orders and portfolio status directly through Alpaca dashboard

---

## 🛠️ Technologies Used

- [x] **FinBERT** - NLP model for financial sentiment
- [x] **Alpaca API** - Market data and commission-free trading platform
- [x] **LumiBot** - Strategy framework (used for automation/backtesting)
- [x] **Transformers** & **PyTorch** - For FinBERT model
- [x] **Matplotlib**, **Seaborn**, **WordCloud** - For visualization

---

## 🎯 Features

✅ Analyze live market headlines using FinBERT  
✅ Buy/Sell stocks automatically using Alpaca API  
✅ View trades in Alpaca’s real-time paper trading dashboard  
✅ Supports interview-ready LumiBot integration  
✅ Clean Jupyter Notebook demo with minimal setup  
✅ No real money involved (Alpaca paper trading safe)

---

## 📊 Alpaca Dashboard

You can view your trades and portfolio activity on the [Alpaca Paper Trading Dashboard](https://app.alpaca.markets/paper/dashboard).

Typical sections shown:

- 📄 **Orders**: All BUY/SELL orders executed by the bot  
- 💼 **Positions**: Current holdings (e.g., SPY)  
- 💰 **Account**: Cash balance, equity, and history  
- 📈 **Activity Log**: Execution details and timestamps

🧪 **Example Interface View**:

![image](https://github.com/user-attachments/assets/6abf9808-8493-4e8f-a0eb-7edef6ba0483)


### 🧠 Workflow

1. **🔍 Fetch News**  
   Retrieves latest headlines for a given stock (e.g., `SPY`) via Alpaca API.

2. **🧠 Analyze Sentiment**  
   Uses `FinBERT` to classify each headline into:  
   `positive`, `negative`, or `neutral`.

3. **📈 Make Decisions**  
   - If strong positive sentiment → **BUY**  
   - If strong negative sentiment → **SELL**  
   - Else → no trade

4. **💼 Execute Orders**  
   Trades are submitted using Alpaca’s paper trading API.

5. **📊 Visualize**  
   - Sentiment pie chart  
   - Word cloud of headlines  
   - Sentiment count bar plot

6. **🤖 Optional LumiBot Mode**  
   Demonstrates integration of LumiBot’s lifecycle methods in a basic `Strategy` class (run when U.S. markets are open).
