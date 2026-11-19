# Day 01 — Define BrokerAI's First Customer

**Date:** 2026-11-19  
**Founder time budget:** up to 5 hours  
**Status:** Draft hypothesis awaiting founder review and user interviews  
**Source of truth:** This repository, `unbu-man/broker`.

## 1. Today's learning goal

A **customer persona** is a research-based description of a group of people with a shared problem, goals, constraints and behavior. A persona is **not proof of demand**. We first write an assumption, then interview real potential users and revise it using evidence.

A **job-to-be-done (JTBD)** describes the progress the customer wants to make. It is more useful than assuming age or income automatically explains customer behavior.

The goal today is to decide **one first target segment** so we do not waste our small founder budget building a broker, trading bots, education, copy-trading, custody and mobile apps at the same time.

## 2. Global vision (draft)

> BrokerAI aims to become a trustworthy international crypto and forex technology platform that helps people understand markets, practice trading, evaluate strategies and manage risk with clear, realistic feedback. We will begin with educational tools and simulated trading, and consider regulated live brokerage services only when jurisdiction-specific permissions, partner arrangements, funding and compliance obligations are satisfied.

**Core markets:** Crypto (BTC/USDT, ETH/USDT) and Forex (EUR/USD, USD/JPY), initially via market-data research and simulation. Stocks/ETFs are deferred.

**Core promise:** *Learn, test and understand risk before committing capital.*

**Never promise:** guaranteed returns, easy profits, zero-risk trading, universally legal access, a reliable prediction of future prices, or instant real-money brokerage availability.

## 3. Proposed primary customer: The risk-conscious self-directed learner

This is a **hypothetical**, not a verified actual user. Call the example persona **Maya**.

| Field | Working hypothesis |
|---|---|
| Segment | Adult who is curious about crypto and/or forex, has limited real-money trading experience and wants to become self-directed |
| Goals | Understand order types and spread/fees; practice trading; assess strategy performance; build risk discipline |
| Current alternatives | Free videos, social trading communities, charting sites, exchange/broker demo accounts, spreadsheets |
| Problems to validate | Confusing terminology; fragmented learning; unrealistic profit screenshots; difficulty comparing real risk and simulated results |
| Desired outcome | Can explain a trade idea, run it in demo, see net P&L and drawdown, and understand why results are uncertain |
| Primary device/language | To be discovered. Start product architecture with English/Khmer localization support, not assumed market-wide demand |
| Trust requirements | Explicit DEMO status; transparent costs and limitations; accurate reconciliation; no misleading backtests; privacy protections |
| Not in initial scope | Custody, deposits, real-money execution, leverage, copy trading, personalized investment recommendations |

**Job to be done:** “When I am considering a crypto or forex trade or strategy, I want to test it with realistic simulated costs and understandable guidance, so I can assess the risks without putting my savings at risk.”

### Five behavioral hypotheses to validate

1. A beginner struggles to distinguish crypto spot trading, forex quoting, and leveraged CFDs.
2. The person would use a guided practice mode at least twice in one week.
3. The person cares about transparent trading costs and losses, not just win rates.
4. An educational assistant would help them understand market concepts, but they would not want it to act as an infallible financial adviser.
5. They would try one paper strategy or simulated signal explanation before paying for a tool.

These are **questions**, not facts; do not put them in an investor pitch as demonstrated findings.

## 4. Secondary segments (not today's target)

| Segment | Need | Why defer it? |
|---|---|---|
| Experienced self-directed trader | Reproducible backtesting, signals, API, demo automation | More advanced tooling and reliable cost models required |
| Professional quant / B2B broker | Infrastructure, APIs, monitoring and custom integration | Requires a different sales process and technical guarantees |
| Retail client seeking a live broker | Account opening, deposits and real-money order execution | Regulatory authorization, custody, compliance and operational controls required |

**Recommended sequence:** beginner simulation → independent trader research features → legally authorized partner/broker services. Do not interpret this as automatic permission to serve retail customers in every country.

## 5. Current problem statement

**Who:** Adult beginner-to-early-intermediate, self-directed crypto/forex learner.

**Situation:** They want to understand how trading and strategies work but find it difficult to tell genuine risk from unrealistic examples.

**Problem:** They lack a coherent, safe way to learn, simulate transactions with realistic costs, and interpret strategy performance.

**Consequence:** They may have poor expectations, confusion about costs and leverage, and inadequate decision processes.

**Opportunity:** Provide risk-first education and verifiable paper-trading tools. No claim of guaranteed improved financial outcomes.

## 6. What we might build for this person

**P0 — required for first paper-trading MVP**

- Clear, accessible market basics in an education area.
- Demo account and virtual portfolio (never mistaken for live money).
- Basic crypto/FX quote data, explicit time and market status.
- Simulated trade entry, history, fees, spread and P&L.
- Explainable risk metrics (drawdown, position sizing and losses) with neutral educational language.

**P1 — after reliable P0**

- Beginner-friendly backtesting and signal explanation.
- Paper-only bot with manual opt-in, position limits and kill switch.
- English/Khmer educational assistant grounded in reviewed content.

**Not MVP:** real deposits or withdrawals, guaranteed AI predictions, profit-share from customer losses, internalized B-Book execution, live crypto derivatives, leveraged FX/CFDs or personalized regulated advice.

## 7. Interview guide — 10 open questions

Interview at least **five real people** who have recently explored crypto/forex learning or demo trading. Do not sell them the product or lead them to a preferred answer.

1. When did you first become interested in crypto or forex, and why?
2. Tell me about the last time you tried to learn a new trading concept.
3. Which sites, apps, or communities did you use, and what was frustrating?
4. Have you ever used a demo or paper-trading account? What happened?
5. How do you currently understand fees, spreads, leverage and potential losses?
6. Describe the last signal or strategy claim you saw. How did you decide whether to trust it?
7. What information would help you decide whether a trading strategy is too risky?
8. What is hardest about tracking simulated trades or reviewing past decisions?
9. If you could change one thing about the tools you use today, what would it be?
10. What have you tried to solve this problem already? Did you spend money or time on it?

**Do not ask leading questions** such as “Would you love our AI trading bot?” Ask for past behavior and specific examples.

### Evidence log (fill after interviews)

| Interview ID | Relevant experience | Actual problem (quote/paraphrase) | Current solution | Severity (1–5) | Evidence that they tried to solve it | Hypothesis revised? |
|---|---|---|---|---|---|---|
| INT-001 | TBD | TBD | TBD | TBD | TBD | TBD |
| INT-002 | TBD | TBD | TBD | TBD | TBD | TBD |
| INT-003 | TBD | TBD | TBD | TBD | TBD | TBD |
| INT-004 | TBD | TBD | TBD | TBD | TBD | TBD |
| INT-005 | TBD | TBD | TBD | TBD | TBD | TBD |

## 8. Validation and decision rules

**Before coding major customer-facing features:**

- Conduct ≥5 non-leading interviews with target-fit adults.
- Record which difficulties happened recently, rather than relying only on opinions.
- At least 3 of 5 should independently describe a related concrete problem **as an early signal only** (not statistical proof).
- Compare the proposed value with existing free/demo tools.
- Revise the persona if evidence contradicts our first guess.
- Select a *first* customer country or user location only after research into local product and marketing restrictions.

A five-person sample is for **qualitative discovery**, not a representative sample of a global market. We must never claim it proves demand, conversion or willingness to pay.

## 9. Founder five-hour session

| Duration | Activity | Deliverable |
|---|---|---|
| 60 min | Learn personas vs JTBD vs market segmentation; read this chapter | Explain all three in your own words |
| 90 min | Review the proposed persona and rewrite it with your assumptions | One-page persona |
| 90 min | Identify five eligible adults to interview; conduct 1–2 initial interviews if practical | Interview notes with consent, no unnecessary identifying data |
| 45 min | Turn interview insights into the top three problems and first product requirements | Revised priorities |
| 15 min | Document changes and GitHub evidence | Commit or issue link |

**Flexible execution:** Interviews can happen over the following days; the task can be marked done once the founder has reviewed the persona, documented a clear first target, and written the interview plan. Actual market validation remains open.

## 10. Day 1 deliverable and acceptance checklist

- [x] Draft vision statement created (founder review pending).
- [x] Proposed primary customer persona documented (not validated).
- [x] Job-to-be-done and problem statement drafted.
- [x] Interview guide and evidence table prepared.
- [ ] Founder confirms or edits the primary persona.
- [ ] Founder selects the top **three** pain points to test first.
- [ ] Founder marks Day 1 complete in the Google Sheet after review.

## 11. Founder decision awaiting confirmation

**Which initial user does the founder most want to serve?**

A. **Beginner learner (proposed):** education + paper trading before advanced bot features.  
B. **Intermediate self-directed trader:** signal research + demo auto bot earlier.  
C. **B2B brokerage customer:** sell platform technology to licensed firms rather than start with individual learners.

Whatever the choice, the first version remains **simulation-only** until regulated activities are appropriately authorized.

## 12. Related planning chapters

- [Global business model](01_global_business_model.md)
- [Crypto and forex MVP scope](07_crypto_forex_scope.md)
- [Five-hour founder daily schedule](09_founder_5_hour_daily_plan.md)
- [Founder sprint 01](05_first_sprint.md)
