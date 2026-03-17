***

### 1. COMPOSITE SCORE
The Composite Score is the ultimate "bottom line" of the dashboard. Instead of forcing the trader to manually weigh conflicting signals (e.g., "Breadth is bad but SPY is going up"), this section does the heavy lifting by aggregating all 6 modules into one master number. 
*Note: The dashboard displays daily change deltas (e.g., `+4.2`) next to key metrics so you can instantly see if the market is expanding or deteriorating compared to yesterday.*

* **The Vibe:** The ultimate traffic light. It tells you exactly how aggressive or defensive you should be with your capital on any given day.
* **How it Works:** It calculates a weighted average of the entire dashboard: Sector Breadth (25%), Index Trend (20%), VIX (20%), MMFI (15%), Factor Regime (10%), and Implied Correlation (10%).

#### HOW THE COMPOSITE SCORE IS CALCULATED (The Weighting)
The Macro Score is a 0 to 100 grade. It is not a simple average; it is a **weighted average** designed to prioritize the most important pillars of the market (Trend and Breadth) while using secondary indicators (like Correlation and MMFI) as confirmation.

**1. Sector Breadth (25% Weight) - *The Heavyweight***
* **Why it's highest:** Under-the-hood participation is the truest measure of market health. The SPY can be skewed by 3 or 4 mega-cap stocks, but Breadth looks at all 27 macroeconomic sectors. If the majority of sectors are "Ripping" or "Turning", this score maxes out.

**2. Index Trend (20% Weight) - *The Foundation***
* **Why it's heavily weighted:** You should never fight the primary trend. This section grants maximum points if the SPY is above its 200-day moving average and moving in a clean, low-chop trend. 

**3. Volatility / VIX (20% Weight) - *The Fear Gauge***
* **Why it's heavily weighted:** Options market pricing is the smartest money in the room. This section awards high points when volatility is low and complacent. It strips away points when fear is expanding. *Note: It awards maximum points at extreme panic levels (> 40 VIX) because of historical contrarian buy-zones.*

**4. MMFI (15% Weight) - *The Swing-Trade Thermometer***
* **Why it's moderately weighted:** Tracking the percentage of stocks above their 50-day moving average tells you if swing breakouts are likely to work today. 

**5. Factor Regime (10% Weight) - *The Institutional Footprint***
* **Why it's lower weight:** This is a confirming indicator. It awards full points if institutional money is hiding in "Risk On" assets and strips points if money is fleeing to "Risk Off" safety assets.

**6. Implied Correlation (10% Weight) - *The Final Polish***
* **Why it's lower weight:** This measures market synchronization. It gives a slight boost to the total score when all factor ETFs are trending together, making stock-picking easier.

**The Math Formula:**
`(Breadth * 0.25) + (Index * 0.20) + (VIX * 0.20) + (MMFI * 0.15) + (Regime * 0.10) + (Correlation * 0.10) = Macro Score (0-100)`

**Metrics & Action Zones:**
* **Macro Score:** The raw 0 to 100 grade of the market.
    * `> 60`: 🟢 Green (Favorable market, tailwinds).
    * `40 to 60`: 🟠 Orange (Mixed market, sideways/choppy).
    * `< 40`: 🔴 Red (Hostile market, headwinds).

* **Action Zone:** Translates the Macro Score into a direct position-sizing and strategy rule.
    * `80 to 100` **(AGGRESSIVE | B/O WORK)**: 🟢 Dark Green. Trade full size, take multiple setups, add aggressively to winning positions. Breakouts have a high win rate.
    * `60 to 79` **(FULL SIZE | B/O WORK)**: 🟢 Light Green. Normal swing trading environment. Standard risk and standard stops.
    * `40 to 59` **(HALF SIZE | THEME B/O)**: 🟠 Orange. The market is transitioning. Cut position sizes in half and only take A+ thematic setups (like tight VCPs). Breakouts are selective.
    * `20 to 39` **(TRAPS ONLY | B/O FAIL)**: 🔴 Light Red. Breakouts will likely fail (Bull Traps). Only buy extreme contrarian setups at 25% position size.
    * `0 to 19` **(CASH / HEDGE | B/O FAIL)**: 🔴 Dark Red. The market is crashing or deeply hostile. Hold cash, do not initiate new longs.

---

### 2. INDEX TREND
This section monitors the broad, surface-level price action of the market (using the SPY as the benchmark) to determine if we are in a clean trend or a messy, untradable chop zone.

* **The Vibe:** "Are we trending cleanly, or are we just chopping traders to pieces?"
* **How it Works:** It maps exactly where the SPY sits within its moving average stack (21 EMA, 50 SMA, 150 SMA, 200 SMA) and uses a custom Chop Index to detect sideways price action.

**Metrics & Brackets:**
* **SPY Trend:** The primary long-term filter.
    * **POWER TREND** (🟢 Green): Full Minervini Stage 2 alignment (Price > 21 > 50 > 150 > 200). The strongest possible trend environment. 
    * **UPTREND** (🟢 Green): Price is above the 21 EMA and 200 SMA, but moving averages aren't perfectly stacked yet. Still highly favorable.
    * **PULLBACK** (🔵 Blue): Price is above the 50 SMA and 200 SMA, but dipped below the fast 21 EMA. A normal, healthy dip. 
    * **DEEP PULLBACK** (🟠 Orange): Price has fallen below the 50 SMA but is holding the 200 SMA. The trend is actively weakening. Reduce size.
    * **BEAR** (🔴 Red): Price is below the 200 SMA. The long-term trend is broken. 

* **Chop Index:** The "cleanliness" of the price action.
    * `< 38.2` **(TRENDING)**: 🟢 Green. Clean, directional price action. Breakouts work easily.
    * `38.2 to 50.0` **(TRANSITION)**: 🟠 Orange. The trend is either just beginning or starting to lose steam.
    * `> 50.0` **(CHOP / CHAOS)**: 🔴 Red. Messy, overlapping daily candles. High probability of getting stopped out (whipsaws). 

* **HTF Weekly:** A Higher Timeframe check to ensure the daily chart isn't lying.
    * `BULLISH`: 🟢 Green. (SPY is above its 20-week EMA).
    * `BEARISH`: 🔴 Red. (SPY is below its 20-week EMA).

---

### 3. SECTOR BREADTH (Druckenmiller Alpha-Physics)
Breadth measures *participation*. A healthy market requires the vast majority of sectors to be moving up together. If the SPY is going up, but only 3 mega-cap tech stocks are carrying it, the Breadth engine will catch the underlying weakness.

* **The Vibe:** "Is the whole army marching forward, or are the generals leading while the troops retreat?"
* **How it Works:** It tracks the Velocity (momentum) and Acceleration (change in momentum) of 27 different macroeconomic ETFs to place them into specific lifecycle phases.

**Metrics & Brackets:**
* **Phase Counts:** Shows exactly where all 27 sectors are in their lifecycle. (Always 🔵 Blue).
    * **Rp (Ripping):** Velocity UP, Acceleration UP. (Strongest phase).
    * **Tu (Turn):** Velocity DOWN, Acceleration UP. (Bottoming out/reversing higher).
    * **Tp (Topping):** Velocity UP, Acceleration DOWN. (Losing steam).
    * **Cr (Crash):** Velocity DOWN, Acceleration DOWN. (Actively selling off).

* **Breadth Score:** A mathematically smoothed 0 to 100 score based on the phases above.
    * `> 60`: 🟢 Green (Healthy participation).
    * `40 to 60`: 🟠 Orange (Mixed participation).
    * `< 40`: 🔴 Red (Poor participation/divergence).

* **Breadth Thrust:** A rare, extremely powerful buy signal indicating massive institutional accumulation.
    * `YES`: 🟢 Green. Triggers when "Fast Breadth" (the percentage of all sectors in the Ripping/Turning phases) violently surges from below 30% to above 60% within a 3-day window.
    * `NO (X bars ago)`: 🔵 Blue. Displays how long it has been since the last thrust.

* **Liquidity (TNX):** Monitors the 10-Year Treasury Yield to see if macroeconomic conditions are favorable.
    * `OK`: 🟢 Green. Yields are falling (below the 21 EMA). Money is cheap, which fuels stock market rallies.
    * `TIGHT`: 🔴 Red. Yields are rising (above the 21 EMA). Debt is expensive, draining liquidity out of risk assets.

---

### 4. FACTOR REGIME (CE Engine)
The Factor Regime is a macroeconomic filter that determines the current "season" of the stock market. Instead of just looking at whether the S&P 500 is going up or down, the Factor Regime looks under the hood to see which specific "types" of stocks (factors) are receiving institutional money.

* **The Vibe:** "Are institutions aggressively buying risk and growth, or are they hiding in safety and dividends?"
* **How it Works:** It tracks the 14-day momentum (Rate of Change) of 15 specific Factor ETFs (like High Beta, Low Volatility, Small Caps, Dividends, Momentum, etc.) and compares them against each other to see what is outperforming. Based on this, it drops the market into one of four buckets (Regimes).

**Metrics & Brackets:**

* **Leading Regime:** The specific macroeconomic "season" we are currently in.
  
* **Goldilocks:** 🟢 Green. The economy is growing at a perfect, sustainable pace. Inflation is tame, and interest rates are friendly. *Outperforms:* Riskier, high-growth assets, High Beta, Small Caps, and Cyclicals. *Underperforms:* "Boring" safety stocks.
* The Vibe: The economy is growing at a perfect, sustainable pace. Inflation is tame, and interest rates are friendly.
* What Outperforms: Riskier, high-growth assets. High Beta (SPHB), Small Caps (IWM), Mid Caps (IWR), and Cyclicals (IYT, IWN).
* What Underperforms: "Boring" safety stocks like Defensives (DEF), Low Volatility (SPLV), and Dividends (SPHD).
  
* **Reflation:** 🟢 Green. The economy is accelerating or bouncing back from a bottom. *Outperforms:* Momentum, High Beta, Small Caps. *Underperforms:* Safety stocks and broad, slow large-caps.
* The Vibe: The economy is accelerating or bouncing back from a bottom. Inflation might be rising a bit, but growth is strong enough to absorb it.
* What Outperforms: Momentum (MTUM), High Beta (SPHB), Small Caps (IWM), and Cyclicals.
* What Underperforms: Safety stocks and broad, slow large-caps.
  
* **Inflation:** 🔴 Red. Prices are rising too fast, interest rates are likely going up, and money is getting tight. *Outperforms:* Safety and Quality. Institutions hide in Low Volatility, Defensives, and Dividends. *Underperforms:* Economically sensitive stocks.
* The Vibe: Prices are rising too fast, interest rates are likely going up, and money is getting tight.
* What Outperforms: Safety and Quality. Institutions hide in Low Volatility (SPLV), Defensives (DEF), Dividends (SPHD), and Quality balance sheets (QUAL).
* What Underperforms: Economically sensitive stocks like Small Caps (IWM) and Transports (IYT).
  
* **Deflation:** 🔴 Red. Economic growth is slowing down or contracting. Demand is falling. *Outperforms:* Pure safety (Defensives, Low Volatility) and sometimes Mega Cap Tech (as a safe-haven bond proxy). *Underperforms:* Small Caps, Cyclicals, and Value.
* The Vibe: Economic growth is slowing down or contracting. Demand is falling.
* What Outperforms: Pure safety. Defensives (DEF), Low Volatility (SPLV), and sometimes Mega Cap Growth (MGK) because mega-tech acts like a safe-haven bond proxy.
* What Underperforms: Small Caps, Cyclicals, and Value stocks.

* **Risk State:** The final verdict based on which regimes are currently scoring the highest.
* `RISK ON` (🟢 Green): Goldilocks or Reflation has the highest score. It is safe to buy breakouts, trade aggressive growth names, and use full position sizing.
* `RISK OFF` (🔴 Red): Inflation or Deflation has the highest score. Breakouts are likely to fail, the market is trapping buyers, and you should be in cash or trading highly defensively.

---

### 5. IMPLIED CORRELATION (CE Engine)
This section measures whether the market's leading factors (like Value, Growth, Size, and Volatility) are aligned and moving together. 

* **The Vibe:** When correlation is high, "a rising tide lifts all boats." Stock picking is on easy mode. When correlation is negative, sectors are fighting each other for capital (hard mode).

**Metrics & Brackets:**
* **ImplCorr Avg:** The average correlation from -1.0 to +1.0.
    * `> +0.10`: 🟢 Green. Highly correlated. Factor tailwinds are strong.
    * `-0.10 to +0.10`: 🔵 Blue. Uncorrelated/Neutral.
    * `< -0.10`: 🔴 Red. Negatively correlated. The market is fragmented.

* **First Green:** A timing tool to catch the exact moment the market synchronizes.
    * `YES`: 🟢 Green. The correlation *just today* crossed above your user-defined threshold (default `0.0`). A strong entry signal.
    * `X ago`: 🔵 Blue. Shows how many days the market has been safely correlated.

---

### 6. MMFI (Market Momentum Filter Index)
A classic swing-trading metric that tracks the exact percentage of stocks in the entire market that are trading above their 50-day moving average.

* **The Vibe:** It acts like an absolute thermometer for the stock market.

**Metrics & Brackets:**
* **MMFI Value & Zone:**
    * `< 20 (CAPITULATION): 🟢 Green. Contrarian buy signal. The market is aggressively oversold and a sharp relief rally is highly likely. The best bounce setups start here.
    * `20 to 40 (BEARISH): 🔴 Red. Bad environment for breakouts. The market is weak, but not washed out enough to buy the dip yet.
    * `40 to 60 (NEUTRAL): 🟠 Orange. No clear edge; the market is struggling to gain footing. It could go either way.
    * `60 to 75 (HEALTHY): 🟢 Green. The "sweet spot" of a bull market move. Breakouts work beautifully and follow through cleanly here.
    * `> 75 (OVERHEATED): 🔴 Red. The market is severely overbought and breadth is stretched too far. Distribution risk is high. Take profits, trail your stops, and do not add new breakout positions.****

* **MMFI Trend:** Is the thermometer rising or falling relative to its moving averages?
    * `RISING`: 🟢 Green. More stocks are reclaiming their 50-day MA today.
    * `FALLING`: 🔴 Red. Stocks are losing their 50-day MA.

---

### 7. VOLATILITY (VIX)
Monitors the CBOE Volatility Index (VIX) to gauge the level of fear, panic, and options-market hedging currently happening on Wall Street.

* **The Vibe:** "Are traders complacent, nervous, or in a state of absolute panic?"

**Metrics & Brackets:**
* **VIX Value & Zone:**
    * `< 20` **(COMPLACENT)**: 🔵 Blue. Normal, low-volatility bull market. Everything is calm.
    * `20 to 30` **(ELEVATED)**: 🔴 Red. Uncertainty is rising. Options are getting expensive.
    * `30 to 40` **(FEAR)**: 🔴 Red. Active, aggressive selloff. Portfolios are taking damage.
    * `> 40` **(EXTREME)**: 🟢 Green. *Contrarian Buy Signal*. Absolute panic has set in. Historically, major market bottoms form here.

* **VIX vs SMA10:** Is fear expanding or contracting right now?
    * `BELOW`: 🟢 Green. Volatility is cooling off (improving).
    * `ABOVE`: 🔴 Red. Volatility is actively expanding (deteriorating).

* **Hedge Signal:** Direct advice based on the VIX.
    * `NO ACTION` (🟢 Green) | `REDUCE SIZE` (🔴 Red) | `HEDGE ACTIVE` (🔴 Red) | `MAX HEDGE` (🟢 Green - preparing to buy the capitulation).

---

### 8. VOLUME ROTATION
Price movements can be faked on low volume, but volume itself cannot be faked. This section follows the footprints of massive institutional money to see exactly where they are placing their bets.

* **The Vibe:** "Follow the whales." If a sector is trading well above its normal volume, Wall Street funds are actively entering or exiting that space.
* **How it Works:** It divides today's volume by the 20-day average volume. The dashboard uses a **1.3x multiple** for Weekly Macro ETFs, and a stricter **1.5x multiple** for Daily SPDRs to filter out normal market noise.

**Metrics & Brackets:**
* **Hot Sectors (W) & (D):**
    * Displays how many sectors are currently experiencing a volume spike out of the total universe.
    * `> 5` (Weekly) or `> 2` (Daily): 🟢 Green. Shows heavy, broad institutional rotation. Else: 🔵 Blue.

* **Top Hot (W) & (D):**
    * Lists the specific tickers with the highest volume spikes, allowing you to see exactly where the money is flowing right now. (Always 🔵 Blue).
    * **The Arrows (Direction):**
        * **▲ (Accumulation):** The sector has a massive volume spike and the price is going *UP*. Institutions are aggressively buying.
        * **▼ (Distribution):** The sector has a massive volume spike and the price is going *DOWN*. Institutions are aggressively dumping/selling.
        * **◼ (Neutral):** Massive volume, but the price hasn't moved. An equal battle between heavy buyers and heavy sellers.

