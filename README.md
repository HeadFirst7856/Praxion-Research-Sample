# Praxion Alpha Lab — Public Research Overview

Praxion Alpha Lab is a privately developed **systematic trading research environment** specializing in:
- **SPX & SPXW microstructure analysis (1-second + 1-minute data)**
- **Systematic 0DTE vertical spread execution**
- **Machine-learning–driven feature engineering**
- **Regime detection**
- **Automated execution (OCO, spread safety, misalignment protection)**
- **Backtesting frameworks for SPX + options**
- **Real-time data engineering (AWS S3)**

This public repository provides a **safe, high-level showcase** of the architecture, strategy design, and bot ecosystem — without exposing proprietary code, API keys, or intellectual property.

---

## 🔍 Core Focus Areas

### **Market Microstructure Research**
- SPX second-level movement  
- Orderflow behavior  
- Volatility clusters  
- Skew/IV dynamics  
- ATM ± strike modeling  

### **Systematic Strategy Engineering**
- SMA crossover systems  
- MRV (VWAP-Zscore mean reversion)  
- TTM Squeeze frameworks  
- Vertical spread optimization  

### **Execution Architecture**
- Combo-only spread execution  
- OCO (Take Profit / Stop Loss) logic  
- Misaligned leg detection  
- Slippage controls  
- Position safety enforcement  

### **Machine Learning Pipelines**
- Regime classifiers  
- Feature catalog (volatility, momentum, microstructure)  
- Signal decay analysis  
- Feature engineering for SPX index + SPXW options  

---

# 📁 Repository Structure

This repo shows the **modular architecture** used across Praxion bots, strategies, and research systems:

├── architecture/
│   ├── system_overview.md
│   ├── data_flow.md
│   ├── execution_flow.md
│   └── bot_orchestration.md
│
├── bots/
│   ├── heartbeat_bot/
│   │   ├── overview.md
│   │   └── connection_management.md
│   ├── spread_guardian/
│   │   ├── overview.md
│   │   ├── oco_management.md
│   │   ├── malformed_spread_detection.md
│   │   └── pnl_digest.md
│   ├── sma_crossover_bot/
│   │   ├── overview.md
│   │   ├── signal_logic.md
│   │   └── execution_rules.md
│   ├── mrv_bot/
│   │   ├── overview.md
│   │   ├── vwap_zscore_logic.md
│   │   ├── adaptive_brackets.md
│   │   └── entry_window.md
│   ├── options_data_logger/
│   │   ├── overview.md
│   │   ├── greeks_capture.md
│   │   └── spx_spxw_sync.md
│   └── regime_monitor/
│       ├── overview.md
│       ├── regime_detection_logic.md
│       └── alerts.md
│
├── strategies/
│   ├── sma_crossover/
│   │   ├── strategy_overview.md
│   │   ├── entry_exit_rules.md
│   │   └── performance_notes.md
│   ├── mrv_strategy/
│   │   ├── strategy_overview.md
│   │   ├── vwap_zscore_rules.md
│   │   ├── time_window.md
│   │   └── risk_model.md
│   ├── ttm_squeeze/
│   │   ├── strategy_overview.md
│   │   ├── histogram_confirmation.md
│   │   └── 50sma_slope_alignment.md
│   └── vertical_spread_framework/
│       ├── spread_selection.md
│       ├── win_loss_barriers.md
│       └── pnl_model.md
│
├── data_pipeline/
│   ├── data_overview.md
│   ├── spx_ingestion.md
│   ├── options_ingestion.md
│   ├── greeks_capture.md
│   └── storage_structure.md
│
├── research/
│   ├── regime_classification/
│   │   ├── regime_overview.md
│   │   ├── features_used.md
│   │   └── examples.md
│   ├── microstructure/
│   │   ├── spx_microstructure_notes.md
│   │   └── option_chain_structure.md
│   └── feature_engineering/
│       ├── feature_catalog.md
│       ├── volatility_features.md
│       └── momentum_features.md
│
└── documentation/
├── terminology.md
├── glossary.md
└── research_philosophy.md

---

# ⚙️ Bot Ecosystem Overview

## **Heartbeat Bot**
Manages:
- API connectivity  
- Reconnect logic  
- Socket stability  
- VPS session survivability  

---

## **Spread Guardian**
Responsible for:
- Vertical spread integrity  
- OCO bracket logic  
- Mid-price validation  
- Misaligned-leg detection  
- Kill-switch & daily loss max  
- Telegram reporting  

---

## **SMA Crossover Bot**
Uses:
- 9 SMA / 50 SMA cross  
- Trend confirmation  
- Combo-only entry  
- Barrier exits  

---

## **MRV Bot**
Implements:
- VWAP / Z-score mean reversion  
- 2:45–3:30 PM entry window  
- Adaptive TP/SL brackets  
- Position sizing logic  

---

## **Options Data Logger**
Captures:
- SPX second-level price  
- 0DTE SPXW option chains  
- Greeks  
- Bid/ask sync  
- ATM ± 8 strikes  

---

## **Regime Monitor**
Tracks:
- Volatility cluster shifts  
- SMA slope changes  
- Momentum states  
- Market regime alerts  

---

# 🧠 Research Framework

Research focuses on:

- SPX microstructure behavior  
- Regime persistence  
- Signal decay curves  
- Feature-quality scoring  
- 0DTE spread asymmetry  
- Time-of-day volatility windows  
- ML-ready features  

Every research module is documented in the **research/** folder.

---

# 🎯 Why This Repo Exists

This public version of Praxion exists to showcase:

- Architectural thinking  
- System design  
- Quant methodology  
- Execution engineering discipline  
- Systematic strategy design  

WITHOUT exposing:

- proprietary code  
- AWS details  
- credentials  
- IBKR logic  
- private data  
- alpha-generating logic  

---

# 🤝 Connect

I’m open to opportunities in:

- Quant Research  
- Systematic Trading  
- Machine Learning for Markets  
- SPX Microstructure  
- Singapore & global hedge funds  

Feel free to reach out or collaborate.
