# arbitrage-bot-n8n
Arbitrage Sentinel is an automated Node.js bot built with n8n. It scans Binance, Bybit, & OKX every 30s to find Cross-Exchange, Triangular, and P2P profit gaps. Unlike basic trackers, it factors in live gas fees, trading commissions, and network latency to deliver validated, actionable signals to Telegram. Precise, scalable, and fast.
Key Technical Features:
Multi-Strategy Engine: Processes Cross-Exchange, Triangular, and P2P-to-Spot arbitrage logic simultaneously.
Hybrid Data Sourcing: Uses exchange-specific REST APIs with a CoinGecko Global Price fallback for 100% uptime.
Precision Profit Modelling: Custom JavaScript nodes calculate net profit by subtracting commissions and network-specific fees.
Smart Confidence Scoring: Ranks opportunities using a weighted algorithm based on margin, speed, and market urgency.
Automated Alerting: Delivers step-by-step execution instructions via Telegram, Email, and Webhooks.                Tech Stack Core: 
n8n Workflow Automation
Runtime: Node.js (Custom JavaScript nodes)
APIs: CoinGecko, Binance, Bybit, OKX, KuCoin, Telegram Bot API                                                     How to Use
Import: Upload the Crypto Arbitrage Signal Platform.json file into your n8n instance.
Configure: Update the "Set Alert Credentials" node with your Telegram Chat ID and Email details.
Deploy: Activate the "Schedule Trigger" to begin 30-second market scans.
