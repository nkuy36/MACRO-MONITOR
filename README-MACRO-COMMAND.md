Here is a highly detailed, comprehensive breakdown for every single section of your Macro Command Center dashboard. I have formatted this exactly like the Factor Regime breakdown so you can easily copy and paste it straight into your documentation!

---

### 1. COMPOSITE SCORE

The Composite Score is the ultimate "bottom line" of the dashboard. Instead of forcing the trader to manually weigh conflicting signals (e.g., "Breadth is bad but SPY is going up"), this section does the heavy lifting by aggregating all 6 modules into one master number.

* **The Vibe:** The ultimate traffic light. It tells you exactly how aggressive or defensive you should be with your capital on any given day.
* **How it Works:** It calculates a weighted average of the entire dashboard: Sector Breadth (25%), Index Trend (20%), VIX (20%), MMFI (15%), Factor Regime (10%), and Implied Correlation (10%).

**Metrics & Brackets:**

* **Macro Score:** The raw 0 to 100 grade of the market.
* `> 60`: 🟢 Green (Favorable market, tailwinds).
* `40 to 60`: 🟠 Orange (Mixed market, sideways/choppy).
* `< 40`: 🔴 Red (Hostile market, headwinds).


* **Action Zone:** Translates the Macro Score into a direct position-sizing rule.
* `80 to 100` **(AGGRESSIVE)**: 🟢 Dark Green. Trade full size, take multiple setups, add aggressively to winning positions.
* `60 to 79` **(FULL SIZE)**: 🟢 Light Green. Normal swing trading environment. Standard risk and standard stops.
* `40 to 59` **(HALF SIZE)**: 🟠 Orange. The market is transitioning. Cut position sizes in half and only take A+ setups (like tight VCPs).
* `20 to 39` **(TRAPS ONLY)**: 🔴 Light Red. Breakouts will likely fail. Only buy extreme contrarian setups (capitulation traps) at 25% position size.
* `0 to 19` **(CASH / HEDGE)**: 🔴 Dark Red. The market is crashing or deeply hostile. Hold cash, do not initiate new longs, or actively hedge.



---

### 2. INDEX TREND

This section monitors the broad, surface-level price action of the market (using the SPY as the benchmark) to determine if we are in a clean trend or a messy, untradable chop zone.

* **The Vibe:** "Are we trending cleanly, or are we just chopping traders to pieces?"
* **How it Works:** It looks at the SPY's position relative to its 200-day moving average, and uses a custom "Chop Index" (measuring a 14-day range vs. Average True Range) to mathematically detect sideways, directionless price action.

**Metrics & Brackets:**

* **SPY Trend:** The primary long-term filter.
* `ABOVE 200`: 🟢 Green (Bull market regime).
* `BELOW 200`: 🔴 Red (Bear market regime).


* **Chop Index:** The "cleanliness" of the price action.
* `< 38.2` **(SUPER TREND / TRENDING)**: 🟢 Green. Clean, directional price action. Breakouts work easily.
* `38.2 to 50.0` **(TRANSITION)**: 🟠 Orange. The trend is either just beginning or starting to lose steam.
* `> 50.0` **(CHOP / CHAOS)**: 🟠 Orange. Messy, overlapping daily candles. High probability of getting stopped out of trades.


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
* **R (Ripping):** Velocity UP, Acceleration UP. (Strongest phase).
* **T (Turn):** Velocity DOWN, Acceleration UP. (Bottoming out/reversing higher).
* **Tp (Topping):** Velocity UP, Acceleration DOWN. (Losing steam).
* **C (Crash):** Velocity DOWN, Acceleration DOWN. (Actively selling off).


* **Breadth Score:** A mathematically smoothed 0 to 100 score based on the phases above.
* `> 60`: 🟢 Green (Healthy participation).
* `40 to 60`: 🟠 Orange (Mixed participation).
* `< 40`: 🔴 Red (Poor participation/divergence).


* **Breadth Thrust:** A rare, extremely powerful buy signal.
* `YES`: 🟢 Green. Triggers when the market goes from heavily "Crashing" to heavily "Ripping/Turning" (>60% of sectors) in just 3 days. Signals massive institutional accumulation.
* `NO (X bars ago)`: 🔵 Blue. Displays how long it has been since the last thrust.


* **Liquidity:** Monitors the 10-Year Treasury Yield (TNX).
* `OK`: 🟢 Green. Yields are falling. Money is cheap, which fuels stock market rallies.
* `TIGHT`: 🔴 Red. Yields are rising. Debt is expensive, draining liquidity out of risk assets.



---

### 4. IMPLIED CORRELATION (CE Engine)

This section measures whether the market's leading factors (like Value, Growth, Size, and Volatility) are aligned and moving together.

* **The Vibe:** When correlation is high, "a rising tide lifts all boats." Stock picking is on easy mode. When correlation is negative, sectors are fighting each other for capital (hard mode).
* **How it Works:** It calculates the 14-day correlation of 15 unique Factor ETFs against the SPY, adjusted by their moving average trends.

**Metrics & Brackets:**

* **ImplCorr Avg:** The average correlation from -1.0 to +1.0.
* `> +0.10`: 🟢 Green. Highly correlated. Factor tailwinds are strong.
* `-0.10 to +0.10`: 🔵 Blue. Uncorrelated/Neutral.
* `< -0.10`: 🔴 Red. Negatively correlated. The market is fragmented.


* **First Green:** A timing tool to catch the exact moment the market synchronizes.
* `YES`: 🟢 Green. The correlation *just today* flipped from negative/neutral into positive territory. A strong entry signal.
* `X ago`: 🔵 Blue. Shows how many days the market has been safely correlated.



---

### 5. MMFI (Market Momentum Filter Index)

A classic swing-trading metric (popularized by Stockbee) that tracks the exact percentage of stocks in the entire market that are trading above their 50-day moving average.

* **The Vibe:** It acts like an absolute thermometer for the stock market.
* **How it Works:** It simply measures the raw percentage (from 0% to 100%) and watches its momentum against short and long-term moving averages.

**Metrics & Brackets:**

* **MMFI Value & Zone:**
* `60 to 80` **(HEALTHY)**: 🟢 Green. The "meat" of a bull market move. Breakouts work beautifully here.
* `< 20` **(CAPITULATION)**: 🟢 Green. *This is a contrarian buy signal*. The market is so aggressively oversold and washed out that a sharp relief rally is mathematically imminent.
* `20 to 60` **(BEARISH / NEUTRAL)**: 🟠 Orange. No clear edge; the market is struggling to gain footing.
* `> 80` **(OVERHEATED)**: 🟠 Orange. The market is severely overbought. Do not initiate new longs; tighten stops and prepare for a sudden pullback.


* **MMFI Trend:** Is the thermometer rising or falling?
* `RISING`: 🟢 Green. More stocks are reclaiming their 50-day MA today than yesterday.
* `FALLING`: 🔴 Red. Stocks are losing their 50-day MA.



---

### 6. VOLATILITY (VIX)

Monitors the CBOE Volatility Index (VIX) to gauge the level of fear, panic, and options-market hedging currently happening on Wall Street.

* **The Vibe:** "Are traders complacent, nervous, or in a state of absolute panic?"
* **How it Works:** It tracks the raw VIX value against standard deviation bands (Bollinger Bands) to detect sudden volatility shocks. *Note: VIX uses contrarian logic at the extremes.*

**Metrics & Brackets:**

* **VIX Value & Zone:**
* `< 20` **(COMPLACENT)**: 🔵 Blue. Normal, low-volatility bull market. Everything is calm.
* `20 to 30` **(ELEVATED)**: 🔴 Red. Uncertainty is rising. Options are getting expensive.
* `30 to 40` **(FEAR)**: 🔴 Red. Active, aggressive selloff. Portfolios are taking damage.
* `> 40` **(EXTREME)**: 🟢 Green. *Contrarian Buy Signal*. Absolute panic has set in. Historically, when the VIX spikes over 40, a major market bottom is being formed.


* **VIX vs SMA10:** Is fear expanding or contracting right now?
* `BELOW`: 🟢 Green. Volatility is cooling off (improving).
* `ABOVE`: 🔴 Red. Volatility is actively expanding (deteriorating).


* **Hedge Signal:** Direct advice based on the VIX.
* `NO ACTION` (🟢 Green) | `REDUCE SIZE` (🔴 Red) | `HEDGE ACTIVE` (🔴 Red) | `MAX HEDGE` (🟢 Green - preparing to buy the capitulation).



---

### 7. VOLUME ROTATION

Price movements can be faked or manipulated on low volume, but volume itself cannot be faked. This section follows the footprints of massive institutional money to see exactly where they are placing their bets.

* **The Vibe:** "Follow the whales." If a sector is trading at double its normal volume, Wall Street funds are actively entering or exiting that space.
* **How it Works:** It divides today's volume by the 20-day average volume. A sector only becomes "Hot" if it crosses a 1.3x multiple (130% of normal volume). It tracks both the 27 Weekly Macro ETFs and the 11 Daily SPDR sectors.

**Metrics & Brackets:**

* **Hot Sectors (W) & (D):**
* Displays how many sectors are currently experiencing a 1.3x volume spike out of the total universe.
* `> 5` (Weekly) or `> 2` (Daily): 🟢 Green. Shows heavy, broad institutional rotation. Else: 🔵 Blue.


* **Top Hot (W) & (D):**
* Lists the specific tickers with the highest volume spikes, allowing you to see exactly where the money is flowing right now. (Always 🔵 Blue).
* **The Arrows (Direction):**
* **▲ (Accumulation):** The sector has a massive volume spike and the price is going *UP*. Institutions are aggressively buying.
* **▼ (Distribution):** The sector has a massive volume spike and the price is going *DOWN*. Institutions are aggressively dumping/selling.
* **◼ (Neutral):** Massive volume, but the price hasn't moved. An equal battle between heavy buyers and heavy sellers.
