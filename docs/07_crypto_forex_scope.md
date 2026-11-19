# Chapter VII — Crypto + Forex MVP Product Scope

**Decision date:** 2026-11-18  
**Founder choice:** Crypto and forex only. **No stocks at MVP.**  
**Current system:** Research and virtual/paper trading; not a regulated brokerage or real-money exchange.

## 1. Market separation

| Dimension | Crypto (phase 1) | Forex (phase 1) |
|---|---|---|
| First paper instruments | BTC/USDT, ETH/USDT | EUR/USD, USD/JPY |
| Initial product | Simulated spot crypto | FX quote and simulated order/position logic |
| Typical session convention | 24 hours, seven days/week (venue-specific interruptions possible) | Business-week sessions, market holidays/rollovers |
| Price source | Identified exchange/venue + timestamp | Identified FX price provider + timestamp, no single consolidated FX tape |
| Quote and base precision | Symbol- and venue-specific increments | Pair- and provider-specific tick sizes |
| Cash/settlement model | Quote currency, virtual balances, fees | Clearly documented virtual FX P&L and conversion assumptions |
| Live legal classification | Trading, brokerage, exchange, custody and tokens/derivatives rules vary | Deliverable FX, rolling spot, margin and CFDs have different legal treatment |
| MVP restriction | No custody, perpetuals or leverage | No real-money dealing, CFD leverage or financial advice |

USDT symbols are **research conventions**, not endorsement of a stablecoin's safety, regulatory suitability or default customer deposit currency.

## 2. Shared software modules

```text
MarketDataProvider -> QuoteNormalizer -> MarketCalendar
                                   |
                              SignalResearch
                                   |
User paper request -> EligibilityGate -> RiskEngine -> SimulatedOrderRouter
                                   |
                       PaperFillEvent -> AuditableLedger
                                   |
                             PortfolioView
```

Each symbol is configured with an asset class, base/quote currencies, minimum order quantity, tick/step precision, quote venue/provider, session rules, and simulated fee model. Never assume crypto and FX pricing are identical.

## 3. Features for version 0.1

1. Virtual account creation with fake starting balance, explicit **DEMO** labels.
2. Clean historical candles and a reproducible quote feed for four starter instruments.
3. Basic buy/sell paper orders and a deterministic simulation engine; no live routing.
4. Orders, fills, open positions and virtual balances kept in a reconciled ledger.
5. Historical backtests with spreads, fees, slippage and market hours.
6. Rule-based risk guards: position caps, trade-rate limits, loss limits, and kill switch.
7. Simple signal engine with confidence/calibration metrics; no claims of guaranteed profit.
8. AI tutor for definitions, risk education and explainable strategy results; no personalized investment advice.

## 4. Deferred features

- Stocks, ETFs, options and securities custody.
- Client deposits, withdrawals, wallets, trading account funding, licensed order execution.
- Margin, perpetuals, futures, liquidation engines, leveraged FX/CFDs and crypto CFDs.
- B-Book market-making/internalization and hybrid live routing until regulatory and conflict-of-interest assessments are documented.
- Copy trading, discretionary portfolio management, personalized signal subscriptions or financial promotion without appropriate authorization.

## 5. Research questions before any live business

1. Which **single initial client market** and **single proposed legal-entity jurisdiction** are realistic?
2. Would the intended product be spot-asset brokerage, an FX dealer service, a CFD product or technology-only tools?
3. Who may hold funds/crypto, price and execute orders, provide liquidity and process withdrawals?
4. What customer protections, AML/KYC/sanctions, capital, segregation, best-execution and disclosure obligations apply?
5. Are retail leveraged products restricted or banned for any intended customer group?
6. Which broker, liquidity provider or exchange partner can lawfully serve selected countries?
7. What are market data licensing and API redistribution constraints?

**Default control:** If legal permission for an activity or country is uncertain, the live feature remains disabled.

## 6. First engineering acceptance tests

- Crypto simulated market data continues over a weekend; FX rejects/queues configured closed-session orders.
- Invalid tick size or quantity step is rejected or deliberately rounded according to documented rules.
- Paper orders are idempotent; identical repeated requests do not double fill.
- No virtual balance goes missing from ledger reconciliation.
- Spread, fees and slippage cause realistic net P&L (no zero-cost backtesting by default).
- Signal research never trains on future candles.
- No UI action or API endpoint can route a real-money order.

## 7. Later instrument candidates
- Crypto: BTC/USD, ETH/USD or venue-specific pairs, subject to data permissions.
- Forex: GBP/USD, AUD/USD and other major FX pairs.
- Gold (XAU/USD) is **not yet included**; it generally introduces additional product/CFD classification questions.

**Next chapter:** finalize customer persona, preferred initial country/partner route, and business viability before implementing the simulator.
