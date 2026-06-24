# Sentinel — AI Financial Intelligence Agent

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Status](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-green)
![Real-Time](https://img.shields.io/badge/System-Real--Time-orange)
![AI](https://img.shields.io/badge/AI-Gemma%204-purple)

Sentinel is a real-time financial intelligence system that detects abnormal market activity and converts raw signals into actionable insights using AI.

Instead of overwhelming users with indicators and charts, Sentinel transforms noisy data into structured intelligence.

---

## 🚀 Features

- Real-time market data ingestion (WebSocket-based)
- Detection of anomalies (volume spikes, RSI extremes, price velocity)
- AI-powered reasoning using Gemma 4
- Structured signal → explanation pipeline
- Modular and extensible architecture

---

## 🧠 System Architecture
WebSocket (Market Data)
↓
Feature Engine (RSI, Volume, Price)
↓
Anomaly Detection Engine
↓
Gemma 4 Reasoning Layer
↓
Insights / API / Dashboard


---

## 📊 Example

### Input Signal
```json
{
  "symbol": "BTCUSDT",
  "volume_spike": 3.1,
  "rsi": 79,
  "price_change": 2.8
}```

AI Output
Strong bullish momentum driven by abnormal volume expansion.
RSI indicates overbought conditions, suggesting continuation is possible but with increasing risk of a pullback.
Watch for sustained volume and resistance breakout.
⚙️ Installation
git clone https://github.com/yourusername/sentinel-ai.git
cd sentinel-ai
pip install -r requirements.txt
▶️ Usage
python main.py

Optional (API mode):

uvicorn app.main:app --reload
🧩 Project Structure
sentinel-ai/
│
├── app/
│   ├── main.py              # FastAPI entrypoint
│   ├── routes.py            # API routes
│
├── core/
│   ├── websocket.py         # Live market data ingestion
│   ├── features.py          # Indicator calculations
│   ├── anomaly.py           # Detection logic
│   ├── gemma.py             # AI reasoning layer
│
├── models/
│   ├── schema.py            # Data schemas
│
├── utils/
│   ├── logger.py
│   ├── config.py
│
├── notebooks/               # Experiments / analysis
├── tests/                   # Unit tests
├── data/                    # Sample data (optional)
│
├── main.py                  # CLI entrypoint
├── requirements.txt
├── README.md
└── LICENSE
🛠 Tech Stack
Python
WebSockets (Binance API)
Pandas / NumPy
FastAPI
Gemma 4
📈 Impact

Sentinel reduces reaction time to market anomalies and improves decision clarity by converting raw data into actionable intelligence.

🔮 Roadmap
 ML-based anomaly detection
 Order book imbalance analysis
 Liquidation data integration
 Real-time alerts (Telegram / Webhooks)
 Backtesting engine
 Multi-asset support
⚠️ Disclaimer!

This project is for research and educational purposes only.
It does not constitute financial advice.

🤝 Contributing

Contributions are welcome.
Open an issue or submit a pull request.

📜 License

MIT License


---
