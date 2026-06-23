# n8n-realtime-crypto-forex-ticker-alerts
Real-time Crypto and Forex price tracking and alert system built on n8n. Fetches live market data and sends instant, formatted updates and volatility alerts via Telegram.
# 📈 Real-Time Crypto & Forex Price Alert System (n8n + Telegram)

A high-frequency, production-ready financial automation workflow built using **n8n**. This system connects with premium market data APIs (like Binance, CoinGecko, or Twelve Data) to fetch **real-time price feeds** for Cryptocurrencies and Forex pairs, automatically broadcasting live ticker updates and custom volatility alerts directly to **Telegram channels or bots**.

## 🚀 Key Features

- **Live Market Fetching:** Periodically polls or listens to live price APIs to capture instant fluctuations in Bitcoin (BTC), Ethereum (ETH), Gold (XAU), or major Forex pairs (EUR/USD).
- **Custom Volatility Triggers:** Features conditional IF-nodes that calculate percentage changes. If a coin pumps or dumps past a certain threshold (e.g., >3% in 5 minutes), it triggers an **Urgent Alert**.
- **Beautifully Formatted Telegram Cards:** Uses custom HTML/Markdown formatting within the Telegram node to send clean, professional trading cards complete with emojis (🟢 for up, 🔴 for down), current price, 24h highs, and volume.
- **Automated Subscription Broadcaster:** Perfect for crypto signal groups or private trading communities looking to automate daily market summaries or instant breakout alerts.

## 🛠️ Built With

- **n8n** (High-Frequency Polling & Advanced Data Transformation)
- **Binance API / CoinGecko API / Financial Data APIs** (For fetching live tickers)
- **Telegram Bot API** (For broadcasting to channels, groups, or private chats)
- **Custom JavaScript** (For mathematical percentage change calculations and currency formatting)

## 📦 How to Deploy This Workflow

1. **Import to n8n:** Download the `trading-alerts-hub.json` file from this repository and upload it into your n8n workspace.
2. **Configure Market API:** Set up your free or premium API keys inside the HTTP Request node for your preferred exchange or market data provider.
3. **Link Telegram Bot:** Create a bot via BotFather on Telegram, grab your Bot Token, add the bot as an Admin to your channel/group, and input the `Chat ID` inside the Telegram node in n8n.
4. **Set Interval Trigger:** Adjust the Cron/Interval node to fetch prices based on your needs (e.g., every 1 minute for high-frequency tracking, or every 1 hour for standard updates).

---
*Developed by Ahmed Tamer - AI Automation Engineer*
