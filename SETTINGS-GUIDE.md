# MACRO COMMAND CENTER - Settings & Configuration Guide

Welcome to the engine room of the Macro Command Center. This guide explains how to configure the indicator's parameters inside the TradingView settings menu to match your exact trading style. 

> **🛑 IMPORTANT:** This document explains *how to configure the settings*. To understand what the dashboard outputs actually mean (and how the color brackets are calculated), you **MUST** read the `README-MACRO-COMMAND.md` file. 

---

### 1. Global Settings
Controls the core heartbeat and visual layout of the dashboard.
* **Indicator Timeframe:** The base timeframe the math uses. Leave this at `240` (4-hour) or `D` (Daily) for optimal swing-trading stability.
* **Table Position / Orientation:** Move the dashboard anywhere on your chart. Use `Vertical` for a standard side-panel, or `Horizontal` to create a top/bottom ticker banner.
* **Text Size:** Adjust to fit your monitor resolution (`Tiny` is recommended for laptops).

### 2. Module Toggles
A checklist that allows you to turn specific dashboard sections on or off to save screen space. Don't trade options? Uncheck the VIX module. Don't care about correlations? Uncheck it. *Note: Disabling a module hides it visually, but the math still runs in the background to calculate your Composite Score.*

### 3. Index Trend
Configure the primary trend and chop parameters.
* **Market Index Ticker:** Defaults to `SPY`. You can change this to `QQQ` if you exclusively trade tech.
* **SMA Length for Bull/Bear:** Defaults to `200`. The ultimate line in the sand for macro regimes. 
* **Chop Thresholds:** The engine mathematically determines if the market is trending cleanly or chopping sideways. You can tweak the Fibonacci default levels (`61.8`, `50.0`, `38.2`) to be more or less sensitive to market noise. 
* **HTF Confirmation:** Sets the Higher Time Frame filter. Defaults to checking if the SPY is above its `1W` (Weekly) `20` EMA.

### 4. Sector Breadth
Fine-tune the Druckenmiller physics engine. 
* **Velocity / Acceleration Lengths:** Defaults to `12` and `3`. Adjusts how fast a sector is categorized as "Ripping" or "Crashing."
* **Volume Weight:** If checked, sectors that are experiencing massive institutional volume spikes are granted 1.5x more weight in your final Breadth Score. 
* **Volume Spike Thresholds:** The multiples required to flag a sector as "Hot." 
   * **Weekly (`1.3` default):** Requires 130% of normal average volume on the macro ETFs.
   * **Daily (`1.1` default):** Requires 110% of normal average volume on the SPDR day-to-day trackers.

### 5. Factor Regime
* **ROC Period:** Defaults to `14`. Measures how fast High Beta, Low Volatility, Small Caps, etc., are moving against each other to calculate the Goldilocks/Reflation/Inflation/Deflation state. 

### 6. Implied Correlation
* **Lengths & KAMA Periods:** The engine uses an adaptive moving average (KAMA) to measure market synchronization. Leave these at default (`14`, `7`, `19`, `8`, `10`) unless you are an advanced quantitative trader.
* **ImplCorr Green Threshold:** Defaults to `0.0`. The exact value the Correlation Average needs to cross above to trigger a "First Green" alignment buy signal. 

### 7. MMFI
* **Short / Long MAs:** Defaults to `10` and `50`. The dashboard uses these averages to determine if the raw percentage of stocks above their 50-day moving average is actively expanding (Rising) or contracting (Falling).

### 8. VIX (Volatility)
Adjust how the indicator interprets fear and complacency.
* **VIX MAs & Bollinger Bands:** Calculates volatility expansions.
* **Thresholds:** * `20.0` (Elevated): The line where normal markets get nervous.
   * `30.0` (Fear): Active distribution.
   * `40.0` (Extreme): The threshold for extreme panic. This triggers a contrarian *buy* signal in the dashboard, as massive VIX spikes historically mark capitulation bottoms.

### 9. Dashboard Colors
Fully customize the aesthetics. 
* **Dashboard Transparency:** Defaults to `15`. Set to `0` for a solid black background, or `100` to make the background invisible (floating text). 
* **Color Palette:** You can change the default Bullish (Green), Bearish (Red), Warning (Orange), and Neutral (Blue) colors to perfectly match your personal TradingView chart theme.
