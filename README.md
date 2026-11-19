# Broker — Global AI Brokerage & Trading Technology

> Founder project · Started 18 November 2026 · Target: a validated platform and launch-readiness decision by November 2027

**Current status: PLANNING / PAPER TRADING ONLY — NOT A LICENSED BROKER.**

## Vision

Build a security-first, AI-assisted trading technology platform designed for **international expansion**, with:

1. A customer-facing trading dashboard and virtual portfolio.
2. Automated **paper-trading** strategies with hard risk limits and a kill switch.
3. Market signal research backed by rigorous, cost-aware testing.
4. An educational assistant for new traders (English/Khmer initially; more languages later).
5. A jurisdiction-aware compliance, onboarding, and execution architecture.
6. An eventual legally approved brokerage or licensed-partner model.

## Initial market scope (founder decision: 18 November 2026)

- **Crypto:** spot-market paper trading first (BTC/USDT and ETH/USDT); crypto futures, perpetuals, margin, custody and real-money exchange integration are out of MVP scope.
- **Forex:** FX price-feed and virtual trade simulation first (EUR/USD and USD/JPY); live retail forex, rolling spot and CFDs remain distinct regulated products subject to review.
- **Stocks and ETFs:** excluded from the first development phase.
- Shared strategy, quote, risk, order and portfolio interfaces will support both markets, while preserving crypto 24/7 trading vs FX weekday schedules, decimal precision, fees, bid/ask spreads, and different settlement/financing conventions.

**We do not guarantee customer profit.** A brokerage should never manipulate order execution to profit from client losses. A-Book, B-Book, or hybrid execution are **research topics**, not authorizations to deal.

## What “global” means

One shared software architecture is possible. **One global brokerage license is not.** Client eligibility, regulated activities, marketing, leverage, custody, investor protection, data handling, tax, and licensing may differ by jurisdiction and product.

The company will select a **first licensed/partner jurisdiction** and separately review each target client market before advertising, onboarding, receiving deposits, providing advice, or executing live orders. Features are enabled only for legally authorized entity–product–country combinations.

## Delivery approach

| Stage | Description | Real-money trading? |
|---|---|---|
| 0 — Research | Product discovery, jurisdiction assessment, business model, fundraising | No |
| 1 — Demo | Market data, backtester, simulated orders, ledgers, paper bots, AI tutor | No |
| 2 — Partner | Explore supervised technology / introducing arrangements with regulated firms | Only with appropriate legal authorization and contracts |
| 3 — Licensed | Regulated live brokerage, if and when capital, approvals and operations permit | Only after approvals |

The **12-month engineering target** is a reliable paper-trading product, validated risk controls, customer research, and a regulator/partner-ready dossier. A live international brokerage is **not guaranteed within 12 months**.

## Read the chapters

- [01 — Global vision and revenue model](docs/01_global_business_model.md)
- [02 — Global regulation and market-entry matrix](docs/02_global_regulatory_strategy.md)
- [03 — Architecture and product scope](docs/03_architecture_and_safety.md)
- [04 — Twelve-month engineering roadmap](docs/04_12_month_roadmap.md)
- [05 — First seven-day sprint](docs/05_first_sprint.md)
- [06 — Decision log](docs/06_decision_log.md)
- [07 — Crypto and forex product scope](docs/07_crypto_forex_scope.md)
- [08 — Solo founder and hiring roadmap](docs/08_founder_team_hiring_plan.md)
- [09 — Founder five-hour daily schedule and first 90 days](docs/09_founder_5_hour_daily_plan.md)
- [10 — Daily task tracking and Google Sheets workflow](docs/10_daily_task_tracking.md)

## Engineering rules

- Initially use **simulated money only**. Never collect deposits, route orders, copy-trade, or give personalized investment advice without relevant authorization.
- No revenue or return guarantees; communicate losses, spreads, fees, and risks transparently.
- Store financial events in an auditable, reconciled ledger. No secret keys, credentials, client PII or real account records in Git.
- Start with Python + FastAPI + PostgreSQL + pytest, and add a TypeScript frontend after validating the core simulator.
- Require documented tests, review and a release note for each milestone.
- Use internationalization (i18n) and country/product eligibility gates from the first design iteration.

## Suggested repository expansion

```text
apps/web/                 # Customer dashboard (future)
services/api/             # FastAPI backend (future)
packages/trading_core/    # Orders, fills, ledger, risk simulation (future)
research/                 # Market data, backtesting, strategies (future)
tests/                    # Unit, integration and financial invariant tests
infra/                    # Docker, staging and CI
docs/                     # Business, legal research and design decisions
```

## Disclaimer

This repository documents a business concept and research software, **not financial advice, authorization or an investment product**. Regulatory summaries are research leads, not legal opinions. Obtain qualified counsel and written regulatory clarity in every intended operating/client jurisdiction.
