# 🛡️ Savantis Glassbox Ledger
**The Public Audit Trail for Savantis Market Intelligence**

Savantis Glassbox Ledger is the transparency initiative for the **Savantis Ecosystem**. It provides a verifiable, immutable, and *a posteriori* historical record of the system's indices and the actual signals broadcasted to our subscribers.

## 📜 Transparency Policy

Data is published in **monthly archives** with a **30-day latency**. This delay protects operational integrity while providing a verifiable audit trail for past performance verification.

## 📂 The Transparency Dataset

This repository hosts the historical log of **individual trade signals** as they were generated and sent. It does not track portfolio performance or aggregated PnL, but rather the raw accuracy and lifecycle of each call.

### 🌪️ Maelstrom (Risk Sentinel)
*Systemic Risk Index.*
*   `ledger/maelstrom/index/`: Historical **ECI** (Extreme Condition Index) scores. The definitive record of the system's risk assessment at any given moment.

### 🟢 Keeper (Invest Signals)
*Strategic Position Management.*
*   `ledger/keeper/signals/`: Historical record of long-term position entries, management adjustments, and exits.

### 🔵 Pathfinder (Swing Signals)
*Trend Navigation.*
*   `ledger/pathfinder/signals/`: Historical record of medium-term directional setups, including entry zones and validation timestamps.

### 🟣 Striker (Scalp Signals)
*High-Frequency Tactics.*
*   `ledger/striker/signals/`: Historical record of rapid-fire tactical opportunities and their immediate outcomes.

## 🛡️ Signal Lifecycle Records

For each signal category, the ledger provides:
*   **Entry:** The exact timestamp and price zone when the signal was broadcast.
*   **Adjustments:** Historical log of any modifications to trade parameters (e.g., Stop Loss adjustments) sent during the trade.
*   **Outcome:** The final result of the individual trade setup (Target Hit, Stop Loss, or Manual Exit) based on market price action.

---
*Savantis Glassbox: Verifiable Intelligence. Trust, but Verify.*
