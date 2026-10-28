# PORTALUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **PORTALUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `PORTALUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `33` months
- **Total Candles:** `1,399,080` 1-minute candles
- **Historical Range:** `2024-02-29 10:00:00` to `2026-10-27 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
PORTALUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── PORTALUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/PORTALUSDT-Historical-Data/main/1m/2026/10/PORTALUSDT_1m_2026-10.csv"
df = pd.read_csv(url)
print(df.head())
```
