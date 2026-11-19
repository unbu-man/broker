# Day 01 — Founder Decisions and Review (Approved)

**Date:** 19 November 2026  
**Founder decision:** Accept the recommended risk-first, phased strategy while preserving the founder's full crypto/forex brokerage ambition.  
**Status:** Strategy approved; customer hypotheses and regulatory permissions still need validation.  
**Repository:** `unbu-man/broker`.

## I. Founder's original direction

The founder wants:
- A **global crypto and forex brokerage** business, not only a Cambodian business.
- Income from useful services for **multiple customer segments**, including people who know nothing about trading, independent and partner-introduced traders, and B2B brokerage firms.
- An **AI bot** for people who want help with trading.
- A **Trading Club** where talented people who lack trading capital can learn and demonstrate skills.
- A mobile + desktop platform with a familiar, accessible brokerage-style experience, intuitive navigation, safety, reliability, and eventually convenient deposits and withdrawals.
- Transparent claims about predictive model performance, without misleading clients.

These are intentions, not evidence of profitability, a working trading model, legal eligibility, capital or customer willingness to pay.

## II. Approved refined company vision

> **BrokerAI will work toward a trusted, globally oriented crypto and forex technology and brokerage ecosystem for learners, self-directed traders, partner-referred clients, and brokerage businesses.** We will pursue sustainable, transparent revenue by delivering useful education, market research, software, risk tools and, only after authorization, brokerage services. Our platform should be responsive on mobile and desktop, simple to navigate, reliable, and clear about trading risks and costs. We will also explore a trading community where capable traders without capital can demonstrate their skills through fair simulated challenges. We will never promise profits, conceal conflicts of interest or rely on pushing unsuitable customers into high-risk trades.

**Positioning:** Education-first and risk-first, but sophisticated tools for experienced traders too.

**Initial instruments:** BTC/USDT, ETH/USDT, EUR/USD, USD/JPY for **research and paper trading only**. Stocks excluded from the first phase.

## III. The customer strategy

| Customer segment | First problem to test | Initial BrokerAI service |
|---|---|---|
| Curious adults with no trading knowledge | Want to understand crypto and forex; may not want to trade | Basic lessons, risk explanations, optional demo |
| Beginners interested in trading | Unsure of orders, spread, fees and losses | Guided virtual account with transparent costs |
| Independent intermediate traders | Hard to review risk and performance | Paper journal, market watch, portfolio and risk metrics |
| Advanced and quantitative traders | Need reliable data and credible signal evaluation | Backtests, simulated strategy API, paper bot with kill switch |
| Partner-introduced traders | Want support without losing personal account control | Own demo account, transparent referral status and consent |
| B2B brokers / platform partners | Need tools and scoped integrations | Research, sandbox APIs and later lawful B2B services |
| Talented individuals without capital | Seek opportunities to build skills and demonstrate results | Trading Club educational community and fair **demo** challenges |

A customer can belong to multiple segments; for example, a partner-introduced complete beginner.

### Target versus eligible

We will **not** monetize legally restricted or unsuitable people through real-money trading merely because they are interested. Non-traders remain eligible for appropriate education and simulation where permitted. Payment, custody, broker execution and customer onboarding are separate regulatory questions for each product and jurisdiction.

## IV. Revenue model — keep it ethical and measurable

**Possible revenue streams to validate:**
1. Optional educational or analytics subscriptions, where lawful and actually useful.
2. Professional strategy-research and backtesting tools sold as software, not profit promises.
3. Licensed B2B software/API subscriptions and integration services.
4. Later, disclosed and legally permitted spreads, commissions or technology service fees from properly authorized brokerage operations.

**Do not assume revenue** from customer losses, guaranteed predictive returns, paid access to profitable bots or a universal right to take deposits. Any A-Book/B-Book/hybrid structure requires specialist legal, execution, conflict-of-interest and financial-risk review.

## V. The first five engineering requirements

These translate the founder's UX, security and performance ideas into verifiable features.

| ID | Requirement | Minimum acceptance test | Phase |
|---|---|---|---|
| F-01 | **Mobile and desktop responsive UI** | Demo pages, order ticket and portfolio are legible and usable across narrow and wide screens with keyboard/accessibility checks | MVP |
| F-02 | **Simple, original broker-style navigation** | Test users can find market watch, virtual order entry, balance, fees, history and help without coaching; do not copy competitors' protected brand/assets | MVP |
| F-03 | **Reliable crypto/FX simulated trading core** | Deterministic order tests, realistic bid/ask and fees, correct decimal arithmetic, duplicate-order protection and reconciled virtual ledger | MVP |
| F-04 | **Explainable learning and honest AI research** | Beginner-safe risk explanations, identifiable market-data sources, holdout-tested signals, confidence and caveats, risk-limited optional paper bot | MVP foundations; advanced phases later |
| F-05 | **Security and operational safety** | Auth, audit trail, secrets controls, backup/restore plan, error handling, monitoring and clear DEMO labeling. Design future deposit/withdrawal controls only; no live funding in MVP | MVP foundations; funding deferred |

### Exness as a design reference

Compare navigation, clarity, supported workflows and usability with existing brokers **without copying brand, proprietary visual assets, source code or implying an affiliation**. Make BrokerAI's own identity and test the interface with users.

### Deposits and withdrawals

The founder's requirement is valid for any eventual brokerage. However, actual real-money funding and withdrawals require licensed entities or partners as applicable, AML/KYC/sanctions checks, reconciled customer-asset records, bank/payment and custodian agreements, fraud controls and complaint handling. **No real-money deposit, withdrawal or order-routing function will be implemented in the demo MVP.**

## VI. AI model claims and testing

The founder's ethical intent, *“tell the truth if the model reaches 90%, not cheat”*, becomes a formal rule:

**Never say only “90% accurate” or “90% profitable” without a precise, verified metric and methodology.**

For any published result record:
- Model version, instrument, timeframe, market-data provider and testing dates.
- Whether “90%” refers to **directional accuracy**, **win rate**, **precision**, **recall**, or another measurable quantity.
- Number of predictions/trades and a realistic uncertainty estimate.
- Train/validation/test boundaries, out-of-sample and walk-forward validation, leakage checks and baseline.
- Fees, spread, slippage, overnight costs where relevant, and whether the test is historical, paper-forward or verified live.
- Net P&L, risk-adjusted metrics, drawdown, volatility, loss distribution and failure cases.

A model can have many winning trades yet lose overall if occasional losses exceed gains. **No model performance metric guarantees customers a profit.** Disclose negative results and model uncertainty just as prominently as positive results.

## VII. Trading Club: innovative idea, cautious rollout

### First version — education and simulated evaluation only
- Lessons, research discussions, demo challenges, transparent rulebook, paper-trade audit and risk-based evaluation.
- Require a meaningful sample size, multiple market regimes, cost-aware scoring and measures that discourage extreme leverage or gambling.
- Do not charge participants fees based on false promises of funding or employment.
- Do not imply the club will allocate real capital after passing a demo test.

### Future research only
A funded-trader or proprietary-trading arrangement would need a defined legal entity, capital, contracts, conflicts assessment, permissions, eligible countries, KYC/AML where applicable, safeguarding, tax and clear payment conditions. Get qualified legal review before any real allocation, prize, performance share or public funding promise.

## VIII. Release sequence for the solo founder

The goal is **one shared product core**, not six separate products built simultaneously.

1. **Core foundation:** crypto/FX market data, instrument definitions, virtual accounts, orders, fee accounting, risk checks, reconciliation and tests.
2. **Demo customer experience:** responsive web UI, simple market watch, trade history, clear costs and risk displays.
3. **Research + AI:** source-grounded education (English and Khmer initially), cost-aware backtests, explained signals, opt-in paper bots and kill switch.
4. **Community + partner sandbox:** Trading Club (demo only), referral attribution with consent, and sandbox B2B reporting/APIs with tenant isolation.
5. **Regulated operation decision:** legal opinions, licensing/partner due diligence, capital, governance, custody/payment arrangements, compliance and independent risk/security reviews **before** any live brokerage.

### First 90 days

A realistic solo-founder target is a credible **tested paper-trading core**, initial discovery interviews, and documented risk/regulatory questions. A production global broker, genuine funded trading club, or guaranteed-profitable bot is **not** a 90-day outcome.

## IX. Open validation questions

- Which people experience the three priority problems in practice, and what tools do they already use?
- Will non-traders actually choose to learn in a demo platform, without pressure to deposit?
- What do experienced traders and potential B2B partners need that existing tools do not provide?
- Does any proposed subscription provide enough measurable value to justify a price?
- What first country/customer market is suitable for a *technology/demo* product, and what licensing route might later be possible for distinct regulated products?
- What legal requirements would apply to the Trading Club's possible future real-money model?

**Customer discovery interviews and legal research remain open. They have not been completed by approving this plan.**

## X. Day 1 decision register

| Decision | Status |
|---|---|
| Crypto + forex; no stocks in initial build | Confirmed |
| Serve a broad set of individual and B2B customer segments | Confirmed |
| Prioritize a shared paper-trading core and risk-first educational UX | Approved product direction |
| Mobile and desktop usability and reliability are core requirements | Approved |
| Real-money beginners' auto bots not in the first release | Approved safety boundary |
| Trading Club starts as learning + demo evaluation | Approved direction |
| No misleading model accuracy or return claims | Approved safety rule |
| Live deposits, withdrawals, custody, execution or funded capital | **Not approved / legally gated** |
| Exact first licensed markets, partners and incorporation | Still open |
| Proof of demand, strategy profitability and product-market fit | Still unverified |

## XI. Next lesson

**Day 2: Competitor and product workflow research.** Evaluate three demo/education/charting or trading platforms as references. Collect evidence about beginner onboarding, mobile/desktop usability, paper trading, display of risks and fees, and product gaps. Decide which five user stories can be built with our available time, and document them in GitHub.

---
**Founder reminder:** This is a business design artifact, not a licensed financial product, performance statement, or marketing permission.
