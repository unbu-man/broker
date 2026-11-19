# Chapter IX — Founder Schedule: Up to 5 Hours per Day

**Date:** 2026-11-18  
**Founder capacity:** Up to **five hours per day**, alongside university studies.  
**Planning assumption:** Five focused sessions weekly = **25 hours/week** (not a promise to work seven days). Weekend time optional; protect study, work, sleep, and recovery.

## 1. Operating principles

1. Build a **demo/paper-trading platform** first: no customer deposits, live execution or promises of profit.
2. Learn the concept, implement it, test it, and document it in the same sprint.
3. Focus on **crypto + forex** (BTC/USDT and ETH/USDT; EUR/USD and USD/JPY) and defer stocks.
4. No full-time hires in the first 90 days; get licensed expert advice on legal questions as needed.
5. When university deadlines reduce capacity, shorten the sprint rather than sacrificing quality, school or health.

## 2. Repeatable daily five-hour session

| Block | Time | Purpose |
|---|---:|---|
| Study | 60 min | Market concepts, Python backend, or financial market regulations |
| Build | 180 min | One small feature, database model, pipeline or interface |
| Test / analyze | 45 min | Unit tests, simulated order reconciliation, data review |
| GitHub journal | 15 min | Commit, short learnings, unresolved questions and next action |
| **Total** | **300 min** | **5 hours** |

A shorter **two-hour fallback** on busy days: 20 min study + 70 min implementation + 20 min tests + 10 min documentation. No penalty for rest days.

## 3. Default weekly allocation (25 hours)

| Session | Focus | Output |
|---|---|---|
| Monday — 5h | Market data and Python | Reproducible data notebook / pipeline |
| Tuesday — 5h | Order simulation, ledger or FastAPI | One passing feature |
| Wednesday — 5h | Market microstructure, statistics, backtesting and tests | Research note + test evidence |
| Thursday — 5h | Refactor, integration, quality and secure architecture | Integrated change + reviewed tests |
| Friday — 5h | Customer research, international compliance research, budget, documentation and weekly retrospective | Decision log + next sprint |

The exact days may move with the university schedule. Keep at least one genuine rest period every week.

## 4. First 90-day goals

### Days 1–30: Fundamentals + first dataset
- [ ] Select first persona, create 10 product requirements, document jurisdiction questions.
- [ ] Establish project structure, local environment, pytest and formatting.
- [ ] Ingest **BTC/USDT** historical data with timestamps, provenance and validations.
- [ ] Add **EUR/USD** as a distinct forex-market feed with sessions and provider information.
- [ ] Write a small data dictionary and publish test results.
- **Exit check:** reproducible datasets; no missing timestamp logic; tests run locally.

### Days 31–60: Trading simulation
- [ ] Create order and instrument schemas with Decimal-based monetary values.
- [ ] Add basic crypto spot simulated buy/sell orders; then adapt FX virtual orders.
- [ ] Implement explicit fees, bid/ask spread and slippage assumptions.
- [ ] Add a testable virtual portfolio and an append-only simulated event log.
- **Exit check:** orders replay deterministically and no duplicate requests cause double fills.

### Days 61–90: Risk + evaluation
- [ ] Add position limits, loss limits, cooldown and manual stop for demo trading.
- [ ] Validate demo cash and positions via reconciliation/invariant tests.
- [ ] Create one simple **rule-based baseline** strategy with in-sample vs out-of-sample split.
- [ ] Compute realistic backtest metrics after transaction costs; document weaknesses.
- [ ] Review the next technical hire/contractor trigger and consult qualified specialists on licensing/market entry.
- **Exit check:** command-line paper trading demonstration, passing test suite, readable README and a go/no-go sprint review.

A 90-day period is about 13 weeks, or roughly **325 planned hours** at 25 hours/week, before breaks/exams. This is an estimate, not a deadline guarantee.

## 5. GitHub sprint definition of done
For every feature:
- User story or engineering goal recorded.
- Implementation and test present (where applicable).
- Financial/data invariants evaluated.
- README / docs updated if behavior or scope changes.
- Commit message describes actual change.
- No secrets, private customer information, licensed data uploads without rights, or misleading performance claims.

## 6. Weekly retrospective template
```markdown
## Week YYYY-WW
Planned hours:
Actual hours:
One thing shipped:
Tests run:
Market/business insight:
What remains uncertain:
Regulatory questions (not conclusions):
One priority next week:
```

## 7. Staffing trigger
Remain founder-led while core research and simulator are manageable. Seek qualified legal counsel early. Consider a part-time experienced engineering reviewer when core correctness/security is beyond available expertise; hire a regulated operations/compliance team only with a concrete authorization route and funding.

**Next practical action:** Start with Project Setup (Python environment, repository structure, pytest, and the BTC/USDT market-data schema).
