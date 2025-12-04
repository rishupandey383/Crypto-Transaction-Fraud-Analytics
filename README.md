# 📊 Crypto Transaction Fraud Analytics
A complete end-to-end analysis pipeline for detecting suspicious crypto transactions across multiple exchanges (Binance, Coinbase, Kraken, KuCoin).  
This project loads, cleans, merges, analyzes, visualizes, and flags anomalies in large-scale crypto transaction datasets.

---

## ⭐ Features
✔ Load datasets from multiple exchanges  
✔ Standardize columns (timestamp, tx_id, from/to address, amount, asset)  
✔ Clean missing or corrupted transaction data  
✔ Generate insights & visual reports  
✔ Detect suspicious/anomalous transactions using ML  
✔ Build an address-transaction network graph  
✔ Rank suspicious wallets using PageRank  
✔ Export all results (CSVs + PNG charts)

---

## 🗂 Dataset Requirements
Place the following CSV files inside a directory (default: `/mnt/data`):

- `binance.csv`
- `coinbase.csv`
- `kraken.csv`
- `kucoin.csv`

Each dataset should contain at least:

- Timestamp column (`timestamp` or `date` or `time`)
- Amount column (`amount`, `value`, or `qty`)
- Transaction ID (`tx_id`, `tx_hash`, etc.)
- Addresses (`from_address`, `to_address`) — optional but recommended
- Asset / currency (`asset`, `currency`)

The script automatically standardizes column names.

---

## 🛠 Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/crypto-fraud-analytics.git
cd crypto-fraud-analytics


pip install pandas numpy matplotlib scikit-learn networkx


python crypto_fraud_analysis.py



