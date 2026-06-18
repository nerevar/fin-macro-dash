# Macro Dashboard - Financial Indicators Reference

## 1. US Equity & Volatility

### S&P 500 (`SP:SPX`)
- **What**: Main US stock market index, 500 largest companies by market cap
- **Why useful**: Primary barometer of US equity market health
- **Exchange**: NYSE/NASDAQ (composite)
- **ISIN**: US78378X1072 (SPY ETF)

### VIX (`TVC:VIX`)
- **What**: CBOE Volatility Index - implied volatility of S&P 500 options for next 30 days
- **Why useful**: "Fear gauge" - spikes during market stress. VIX > 30 signals high fear, < 15 complacency
- **Exchange**: CBOE

### VVIX (`CBOE:VVIX`)
- **What**: Volatility of VIX - implied volatility of VIX options
- **Why useful**: Measures uncertainty about uncertainty itself. Extreme readings signal potential regime changes

---

## 2. US Fixed Income & Rates

### 10-Year Treasury Yield (`TVC:US10Y`)
- **What**: Yield on US 10-year government bonds
- **Why useful**: Benchmark for mortgage rates, corporate borrowing. Key indicator of inflation expectations and economic outlook
- **Current context**: Rising yields = market expects higher rates/inflation; falling = flight to safety

### 2-Year Treasury Yield (`TVC:US02Y`)
- **What**: Yield on US 2-year government bonds
- **Why useful**: Most sensitive to Fed policy expectations. 2Y > 10Y = yield curve inversion = recession signal

### 30-Year Treasury Yield (`TVC:US30Y`)
- **What**: Yield on US 30-year government bonds
- **Why useful**: Long-term inflation/growth expectations. Key for pension funds and long-duration assets

### Fed Funds Rate (`FRED:FEDFUNDS`)
- **What**: The interest rate at which banks lend reserves to each other overnight (set by Federal Reserve)
- **Why useful**: THE policy rate. Drives all other interest rates. Higher = tighter monetary conditions
- **Data source**: FRED (Federal Reserve Economic Data)
- **Update frequency**: After each FOMC meeting (~8x/year)

### 10Y-2Y Spread (`FRED:T10Y2Y`)
- **What**: Difference between 10-year and 2-year Treasury yields
- **Why useful**: Classic recession predictor. Negative spread (inversion) has preceded every US recession since 1969
- **Current context**: Watch for re-steepening after inversion as signal recession may be imminent

### MOVE Index (`TVC:MOVE`)
- **What**: Merrill Lynch Option Volatility Estimate - implied volatility of Treasury options
- **Why useful**: "VIX for bonds". Spikes signal fixed income market stress. Important during rate hiking/cutting cycles

---

## 3. Currencies

### EUR/USD (`FX:EURUSD`)
- **What**: Euro vs US Dollar exchange rate
- **Why useful**: Most traded currency pair globally. Reflects relative US/Europe economic strength

### USD/JPY (`FX:USDJPY`)
- **What**: US Dollar vs Japanese Yen
- **Why useful**: Key carry trade pair. Yen strengthens during risk-off (safe haven). BOJ policy shifts cause major moves

### DXY Index (`TVC:DXY`)
- **What**: US Dollar Index - weighted average vs basket of 6 major currencies (EUR 57.6%, JPY 13.6%, GBP 11.9%, CAD 9.1%, SEK 4.2%, CHF 3.6%)
- **Why useful**: Single measure of USD strength. Strong dollar = headwind for commodities and EM; weak dollar = tailwind

### THB/USD (`FX_IDC:THBUSD`)
- **What**: Thai Baht vs US Dollar
- **Why useful**: Relevant for Thai exposure/living costs, emerging Asia currency indicator

---

## 4. Commodities

### Gold (`TVC:GOLD`)
- **What**: Spot gold price in USD per troy ounce
- **Why useful**: Ultimate safe haven. Hedge against inflation, currency debasement, geopolitical risk
- **ISIN**: GLD ETF - US78463V1070
- **Current context**: War premium, central bank buying, de-dollarization trend

### Silver (`TVC:SILVER`)
- **What**: Spot silver price in USD per troy ounce
- **Why useful**: Industrial + precious metal. Higher beta than gold. Gold/silver ratio useful for relative valuation

### Oil WTI (`NYMEX:CL1!`)
- **What**: West Texas Intermediate crude oil front-month futures
- **Why useful**: US benchmark crude. Key input for inflation, energy costs, geopolitical risk pricing
- **Exchange**: NYMEX (CME Group)
- **Current context**: Iran tensions directly impact oil supply/risk premium

### Oil Brent (`TVC:UKOIL`)
- **What**: Brent crude oil price - international benchmark
- **Why useful**: Global benchmark (vs WTI = US). Brent-WTI spread indicates regional supply dynamics
- **Exchange**: ICE

### Natural Gas (`NYMEX:NG1!`)
- **What**: Henry Hub natural gas front-month futures
- **Why useful**: Key energy commodity. Seasonal patterns, LNG export impact, Europe energy security
- **Exchange**: NYMEX

### Copper (`COMEX:HG1!`)
- **What**: Copper futures price
- **Why useful**: "Dr. Copper" - industrial bellwether. Rising copper = economic expansion expectations
- **Exchange**: COMEX (CME Group)

---

## 5. Crypto

### Bitcoin (`BITSTAMP:BTCUSD`)
- **What**: Bitcoin price in USD
- **Why useful**: Digital gold narrative, risk-on/off indicator, institutional adoption tracker
- **Exchange**: Bitstamp (also tracked on Coinbase, Binance etc.)

### Ethereum (`BITSTAMP:ETHUSD`)
- **What**: Ethereum price in USD
- **Why useful**: Platform for DeFi/smart contracts. ETH/BTC ratio shows altcoin risk appetite

### BTC Dominance (`CRYPTOCAP:BTC.D`)
- **What**: Bitcoin's market cap as percentage of total crypto market cap
- **Why useful**: Rising = risk-off in crypto (money flows to BTC); falling = altcoin season, more speculative

---

## 6. Russia & CIS

### MOEX Index (`MOEX:IMOEX`)
- **What**: Moscow Exchange main index (IMOEX) - ruble-denominated
- **Why useful**: Primary indicator of Russian equity market health
- **Exchange**: MOEX (Moscow Exchange)

### USD/RUB (`MOEX:USDRUB_TOM`)
- **What**: US Dollar to Russian Ruble exchange rate (tomorrow settlement)
- **Why useful**: Russian economy health indicator, sanctions impact tracker
- **Exchange**: MOEX, TOM (T+1 settlement)

### EUR/RUB (`MOEX:EURRUB_TOM`)
- **What**: Euro to Russian Ruble exchange rate
- **Why useful**: EU-Russia economic relationship indicator

### CNY/RUB (`MOEX:CNYRUB_TOM`)
- **What**: Chinese Yuan to Russian Ruble exchange rate
- **Why useful**: Reflects Russia-China trade relationship, de-dollarization trend
- **Current context**: Growing importance as Russia shifts trade to China

### RGBI Bond Index (`MOEX:RGBI`)
- **What**: Russian Government Bond Index - price index of OFZ (federal loan bonds)
- **Why useful**: Russian fixed income market health. Sensitive to CBR rate decisions, sanctions, fiscal policy
- **Exchange**: MOEX

### Gold/RUB (`MOEX:GLDRUB_TOM`)
- **What**: Gold price denominated in Russian Rubles
- **Why useful**: Ruble-based gold price for RUB portfolio hedging. Popular on MOEX for retail investors
- **Exchange**: MOEX

---

## 7. European Indices

### DAX (`XETR:DAX`)
- **What**: Germany's main stock index - 40 largest companies on Frankfurt Stock Exchange
- **Why useful**: Europe's largest economy. Export-heavy, sensitive to global trade and China demand
- **Exchange**: XETRA (Frankfurt)
- **ISIN**: DE0008469008

### FTSE 100 (`FTSE:UKX`)
- **What**: UK's main stock index - 100 largest companies on London Stock Exchange
- **Why useful**: GBP-denominated, commodity/financial heavy. Post-Brexit UK economic barometer
- **Exchange**: LSE

### Euro Stoxx 50 (`TVC:SX5E`)
- **What**: Eurozone blue-chip index - 50 largest companies across 11 eurozone countries
- **Why useful**: Best single measure of eurozone equity performance
- **Exchange**: STOXX (Eurex)

### CAC 40 (`EURONEXT:PX1`)
- **What**: France's main stock index - 40 largest companies on Euronext Paris
- **Why useful**: France is eurozone's #2 economy. Luxury sector heavy (LVMH, Hermes)
- **Exchange**: Euronext Paris

---

## 8. Asian Indices

### Nikkei 225 (`TVC:NI225`)
- **What**: Japan's main stock index - 225 largest companies on Tokyo Stock Exchange
- **Why useful**: Asia's most developed market. BOJ policy and yen movements create major opportunities
- **Exchange**: TSE (Tokyo)

### Hang Seng (`TVC:HSI`)
- **What**: Hong Kong's main stock index
- **Why useful**: Gateway to Chinese equities. Sensitive to China regulation, US-China tensions, property crisis
- **Exchange**: HKEX

### Shanghai Composite (`SSE:000001`)
- **What**: China's main stock index - all shares on Shanghai Stock Exchange
- **Why useful**: Direct China domestic equity market indicator. Driven by government policy and stimulus
- **Exchange**: SSE (Shanghai)

### KOSPI (`KRX:KOSPI`)
- **What**: South Korea's main stock index
- **Why useful**: Tech/semiconductor heavy (Samsung, SK Hynix). Global chip cycle indicator
- **Exchange**: KRX (Korea Exchange)

---

## 9. Global ETFs

### IWDA (`LSE:IWDA`)
- **What**: iShares Core MSCI World UCITS ETF - tracks developed world equities
- **Why useful**: Single-ticket diversified global exposure. ~70% US, rest is developed ex-US
- **Exchange**: LSE (London)
- **ISIN**: IE00B4L5Y983
- **TER**: 0.20%

### EEM (`AMEX:EEM`)
- **What**: iShares MSCI Emerging Markets ETF
- **Why useful**: Broad emerging market exposure. ~30% China, significant India, Taiwan, Korea
- **Exchange**: NYSE Arca
- **ISIN**: US4642872349
- **TER**: 0.70%

---

## 10. Macro Data

### US National Debt (`FRED:GFDEBTN`)
- **What**: Total public debt of the United States federal government
- **Why useful**: Fiscal sustainability indicator. Rapid growth raises concerns about future inflation and dollar confidence
- **Data source**: FRED (US Treasury data)
- **Update frequency**: Quarterly
- **Current level**: ~$36 trillion (2025)

### 10Y Breakeven Inflation (`FRED:T10YIE`)
- **What**: Difference between 10Y nominal Treasury yield and 10Y TIPS yield
- **Why useful**: Market's expectation of average inflation over next 10 years. Rising = inflation fears, falling = disinflation
- **Data source**: FRED
- **Normal range**: 2.0-2.5% (around Fed's target)

### HY Credit Spread (`FRED:BAMLH0A0HYM2`)
- **What**: ICE BofA US High Yield Index Option-Adjusted Spread (OAS)
- **Why useful**: Measures stress in corporate credit. Widening = increased default risk/recession fears. Tightening = risk-on
- **Data source**: FRED (ICE/BofA data)
- **Recession signal**: Spread > 500-600 bps historically signals recession

### Baltic Dry Index (`INDEX:BDI`)
- **What**: Shipping cost index for dry bulk cargo (iron ore, coal, grain) on major sea routes
- **Why useful**: Leading indicator of global trade and economic activity. Cannot be speculated easily - pure supply/demand
- **Note**: Highly volatile, seasonal patterns

---

## Correlation & Anti-Correlation Pairs to Watch

| Pair | Expected Relationship | What Divergence Means |
|------|----------------------|----------------------|
| S&P 500 vs VIX | Strong inverse | Divergence = potential trend change |
| Gold vs DXY | Inverse (usually) | Both rising = extreme stress |
| Oil vs RUB | Positive (Russia = oil exporter) | Decoupling = sanctions effect |
| 10Y yield vs Gold | Inverse (real rates) | Rising yields + rising gold = inflation fear |
| BTC vs S&P 500 | Positive (risk-on) | Decoupling = narrative shift |
| DXY vs EM currencies | Inverse | Strong dollar crushes EM |
| Copper vs S&P 500 | Positive (growth) | Copper leading = early cycle signal |
| 10Y-2Y spread vs stocks | Complex | Inversion precedes recession by 6-18mo |
| VIX vs MOVE | Correlated in crises | MOVE leading VIX = bond-driven crisis |
| Gold vs BTC | Debated | Both rising = monetary debasement trade |
