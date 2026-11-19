# Day 01 — Define BrokerAI's Customers and Their Problems

**Date:** 19 November 2026  
**Study/build time:** Up to five focused hours  
**Project:** BrokerAI — Global Crypto + Forex (stocks deferred)  
**Stage:** Product discovery; **education and simulated/paper trading only**  
**Decision from founder:** We eventually want to serve **all relevant customer groups**, including people who know nothing about trading, independent traders, partner-referred individuals, and brokerage businesses. That does **not** mean every feature must be built in the first release.

## Objective

By the end of Day 1, we should be able to answer:

1. **Who can benefit from BrokerAI?**
2. **What problem does each group have?**
3. **Which shared features solve those problems?**
4. **What is the first user journey we will build with a solo founder's 25-hour/week capacity?**
5. **Which functions require licensing or other legal permissions and therefore remain disabled?**

The initial customer segmentation is a **hypothesis**. Later interviews and usage tests must validate or change it.

## 1. Learn the fundamentals — 60 minutes

Understand and explain in your own words:

- **Customer segment:** people or organizations sharing similar needs (e.g., first-time learners, active traders, brokerage firms).
- **Persona:** a specific, evidence-backed description of a representative customer, including problems and workflows.
- **Job to be done (JTBD):** the progress a customer is trying to achieve, often framed as: “When [situation], I want [action], so that [outcome].”
- **Target vs eligible:** we may welcome almost anyone to **learn**, while real-money services may be restricted by age, jurisdiction, regulation, suitability, onboarding/KYC or product type.

Write 1–2 sentences defining each term without using our product name.

## 2. Map all intended customer groups — 90 minutes

| Group | What they want | Working problem hypothesis | Appropriate early experience |
|---|---|---|---|
| **A. Curious non-traders** | Understand crypto/forex before deciding whether trading is for them | Unfamiliar terminology; difficulty recognizing losses, scams and unrealistic claims | Free explanations, risk education and optional guided demo |
| **B. Complete beginners** | Learn how markets and basic orders work | Confusion about prices, spreads, fees and risk | Learning path + virtual account |
| **C. Intermediate independent traders** | Analyze markets and improve their process | Hard to track costs, risk and results reliably | Charts, journal, realistic paper trades, signal explanations |
| **D. Experienced independent traders** | Test strategies and automation | Backtests may omit costs and have look-ahead bias | Research tools, reproducible backtests and paper bot with kill switch |
| **E. Partner-referred individuals** | Access the same tools through a trusted partner | They may need optional partner support without losing account autonomy | Own demo account, clear referral relationship and consent controls |
| **F. Brokers and B2B partners** | Serve eligible clients and integrate infrastructure | Custom platforms, risk tools and reporting are expensive | Demo organization portal, sandbox APIs and scoped reporting |

**Important:** A beginner might also be a partner-referred individual; experience, referral source and legal eligibility are separate attributes. “Non-target” is not a label for someone who lacks trading knowledge. A visitor who decides not to trade is a legitimate outcome of good education.

**Your task:** For each group, add one specific example of a customer problem **without presenting assumptions as proven facts**. Mark each example as `hypothesis` until verified.

## 3. Draft the product promise and boundaries — 45 minutes

### Working vision

> BrokerAI aims to be a trustworthy global crypto and forex technology platform where anyone can learn how trading works, experienced individuals can research and practice strategies, and eligible brokerage partners can eventually use related business tools. We will start with transparent education, risk analytics and paper trading. Live services will require authorization for the entity, product and customer's jurisdiction.

### What we must never promise

- Guaranteed profit, accurate future-price predictions or “risk-free” trading.
- That using the AI bot is necessary to become financially secure.
- That referring or educating someone automatically allows us to accept their money or execute their orders.
- That every country permits our products or that a single license allows global brokerage.
- That a referring broker automatically controls a customer's account, trades or data.

**Your task:** Rewrite the vision in 3–5 sentences and list at least three non-negotiable trust principles.

## 4. Choose a shared MVP journey (without rejecting other segments) — 75 minutes

**Recommended first build order:**

```text
Visitor (any experience level)
  → Education + honest risk explanation
  → Optional individual DEMO account
  → Crypto/FX virtual orders and transparent P&L
  → Risk dashboard + trading journal
  → Optional demo signal research / paper bot
  → Later: consent-based partner affiliation and B2B sandbox
  → Live brokerage only if separately authorized
```

This is **sequencing**, not a decision to serve only beginners. The shared paper-trading engine can eventually power advanced and partner interfaces.

**Your task:** Write the five most important capabilities for the earliest usable version. Proposed:

1. Learn the fundamentals of crypto/forex and their risks.
2. Open a clearly labeled simulated-money account.
3. Place basic virtual orders and see bid/ask prices and fees.
4. Understand position exposure, losses, equity and drawdown.
5. Review trade history and simple research signals with limitations.

Also decide what is **not** part of version 0.1: real deposits, withdrawals, live execution, leveraged retail CFDs, crypto derivatives, personalized advice, discretionary account management or custody.

## 5. Prepare customer discovery — 30 minutes

Create a list of at least **six possible adult interview participants** spanning different experiences (for example, two curious non-traders, two individual traders and two brokerage/partner industry contacts, if accessible). Do not publish names or personal information in GitHub.

Ask open-ended questions, not sales questions:

1. What makes you interested in crypto/forex, or what do your clients ask for?
2. What was the last trading-related task you attempted?
3. Which websites/apps did you use? What confused or frustrated you?
4. How do you judge trading costs, losses and risks?
5. What would you want from a paper-trading or educational tool?
6. If working with a broker, what customer data and controls should that broker be allowed to see?

**Interview results are not required to finish today's document.** They are follow-up validation tasks, not permission to claim that these personas are proven.

## 6. Document and save — 20 minutes

Write a short `docs/day_01_customer_notes.md` (or use this document as a working log):

```markdown
# My Day 1 decisions

## BrokerAI vision
[3–5 sentences]

## Customer groups included
A / B / C / D / E / F (all groups in long-term scope)

## Top 3 problems to validate
1.
2.
3.

## MVP first user journey
[Visitor → Learn → Paper trading → Review risk]

## Five must-have features
1.
2.
3.
4.
5.

## Three things we will NOT promise
1.
2.
3.

## Open questions for real interviews
1.
2.
```

Add a GitHub commit and record its link in the **Daily Tasks** tracker.

## Completion checklist

- [x] Founder confirmed the long-term multi-segment strategy.
- [x] Draft segment map covering curious non-traders, beginners, active traders, partner-referred customers and brokers.
- [x] Initial product vision, boundaries and first demo journey proposed.
- [ ] Founder writes their own vision paragraph.
- [ ] Founder identifies top three unproven customer problems.
- [ ] Founder agrees on first five MVP capabilities.
- [ ] Interview candidates identified; actual customer interviews still pending.

**Done for Day 1 means your hypotheses are clearly documented—not that all six markets have been validated or every customer feature has been built.**

## Related project references

- [Global business model](01_global_business_model.md)
- [Crypto/forex product scope](07_crypto_forex_scope.md)
- [Founder five-hour plan](09_founder_5_hour_daily_plan.md)
- [First sprint](05_first_sprint.md)
