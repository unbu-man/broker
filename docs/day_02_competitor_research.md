# Day 02 — Competitor Research and BrokerAI User Stories

**Date:** 20 November 2026
**Founder study time:** 5 hours
**Project:** BrokerAI crypto + forex — education and **paper trading only**.
**Status:** Official-source desk research complete; hands-on ratings and customer validation remain open.

## Goal

Study three relevant trading products, identify how they present markets, risk, demo mode and user experience, and translate observations into **five buildable BrokerAI requirements**. We will develop an original product, not copy another company's code, artwork or branding.

## Competitor comparison from official documentation

| Platform | Why we study it | Confirmed documented functions | What BrokerAI can learn |
|---|---|---|---|
| Exness | Broker-style experience, forex, mobile and desktop | Demo accounts; Exness Trade app; browser Exness Terminal; bid/ask and balance/equity/order history | Distinguish DEMO from live; make trade forms and account history clear |
| TradingView | Charting and paper trading for crypto and forex | User-facing Paper Trading account; chart-based analysis; order tickets and practice positions | Chart-to-order workflows and understandable risk/performance reporting |
| Binance Spot + Academy | Crypto market structure and education | BTC/USDT spot trading guide, market/limit orders; independent developer API and Spot Testnet | Pair precision, order types and contextual beginner education |

**Important:** Binance Spot Testnet is a **developer test environment**, not proof that all retail Binance users can open the same type of demo account. Exness demo is broker-specific; TradingView offers its own paper-trading service. Available features and access conditions may vary by country, account and product.

### Official sources inspected on 20 Nov 2026

- Exness demo: https://www.exness.com/demo-trading-account/
- Exness Terminal guide, updated 2026-08-06: https://get.exness.help/hc/en-us/articles/360013671560-Exness-Terminal-Trading-guide
- Exness mobile account help: https://get.exness.help/hc/en-us/articles/360014872440-Exness-Trade-Creating-trading-accounts
- TradingView Paper Trading: https://www.tradingview.com/support/solutions/43000516466-paper-trading-main-functionality/
- TradingView features: https://www.tradingview.com/features/
- Binance Academy spot guide, updated 2026-06-18: https://academy.binance.com/en/articles/your-guide-to-binance-spot-trading
- Binance developer introduction: https://developers.binance.com/en/docs/introduction
- Binance Spot Testnet docs: https://developers.binance.com/en/docs/products/spot/testnet/rest-api

**Evidence limitation:** Official websites can substantiate feature claims, but not comparative usability, customer satisfaction, execution speed or product suitability. We have not logged in, personally tested mobile apps or verified local eligibility. Mark untested criteria **N/V**, not zero.

## Five-hour assignment

| Time | Your task | Output |
|---|---|---|
| 30 min | Read our goal and the eight official sources | Understand what we can compare fairly |
| 60 min | Study Exness account/demo and terminal help | Five notes on demo, quotes, fees, history and mobile/web |
| 60 min | Study TradingView paper trade documentation | Five notes on charts, order ticket, paper results and research |
| 60 min | Study Binance Spot & Academy | Five notes on BTC/USDT, market/limit orders, risks and test environments |
| 60 min | Complete scorecard and revise user stories | Evidence-backed comparison with N/V where applicable |
| 30 min | Write 3 observations, 3 opportunities, and save to GitHub | Evidence link and short reflection |

**No real deposits or live trades are necessary or requested.** It is acceptable to examine public pages instead of opening trading accounts.

## Personal inspection scorecard (not rated yet)

Scoring:
- **0** = Did not find it during a genuine test (this does not prove it is absent).
- **1** = Difficult for a beginner.
- **2** = Understandable with some difficulty.
- **3** = Clear and intuitive.
- **N/V** = Not personally verified.

| Test | Exness | TradingView | Binance | BrokerAI improvement |
|---|---|---|---|---|
| Can a novice find a place to start? | N/V | N/V | N/V | |
| DEMO and live functions are distinguishable | N/V | N/V | N/V | |
| Market/symbol discovery is clear | N/V | N/V | N/V | |
| Order type and quantity are understandable | N/V | N/V | N/V | |
| Spread/fees and risks are understandable | N/V | N/V | N/V | |
| Mobile and desktop layouts are usable | N/V | N/V | N/V | |
| Trade history and net P&L are easy to locate | N/V | N/V | N/V | |
| Help and beginner learning are accessible | N/V | N/V | N/V | |

Don't declare a winner before completing the scorecard through firsthand observation.

## Initial five BrokerAI user stories

| ID | As a user | I want | Initial acceptance test |
|---|---|---|---|
| US-01 | Curious adult or beginner | To learn trading basics and risks before deciding to practice | Clear Learn and Try Demo paths; no deposits or income promises |
| US-02 | Independent or partner-referred trader | To use a consistent paper account on phone and computer | DEMO balance, markets, order ticket and history readable at 375px and 1280px |
| US-03 | Paper trader | To preview trade costs before placing an order | Valid bid/ask, fees, precision; no duplicate fills and insufficient virtual cash rejected |
| US-04 | Self-directed trader | To review my demo performance honestly | Reconciled virtual balances, realized/unrealized P&L, costs and drawdown |
| US-05 | Learner or advanced trader | To understand signal or bot limitations | Signal metric/test dates shown; opt-in paper bot has hard risk limits and kill switch |

**Later, not MVP:** real deposits, withdrawals, live execution, leverage, funded trader program, personalized advice, broker access to individual trading accounts and real-money strategy automation. Partner/B2B sandbox will require consent and data isolation.

## Our proposed demo navigation

```text
BrokerAI DEMO
├── Learn (Crypto, Forex, Risks, Glossary)
├── Markets (BTC/USDT, ETH/USDT, EUR/USD, USD/JPY)
├── Paper Trade (Preview → Submit → History)
├── Portfolio (Virtual balance, Costs, P&L, Drawdown)
├── Research (Backtests, Signals, Paper Bot — later)
├── Trading Club (Demo learning/challenges — later)
└── Account / Help
```

Use one common market-data/order/ledger/risk core while showing simpler explanations to beginners and advanced analysis to experienced users.

## Your notes — fill after inspection

**Exness:** Three real observations: __, __, __. One improvement for BrokerAI: __.

**TradingView:** Three real observations: __, __, __. One improvement for BrokerAI: __.

**Binance:** Three real observations: __, __, __. One improvement for BrokerAI: __.

**Five user stories to prioritize:** US-__ → US-__ → US-__ → US-__ → US-__.

## Completion

- [x] Three platform references chosen and official docs reviewed.
- [x] Eight evaluation criteria drafted; do not interpret blank ratings as zero.
- [x] Five proposed user stories documented.
- [ ] Founder personally inspects available pages/screens and fills ratings.
- [ ] Founder describes three verified observations and three product hypotheses.
- [ ] Founder selects first development priority and records it in GitHub.
- [ ] Founder marks Day 2 complete in Google Sheet **after finishing**.

**Next:** Day 3 will research a shortlist of potential legal jurisdictions and client-market restrictions; no assumption of a single global brokerage license.
