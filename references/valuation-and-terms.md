# Valuation, Return, Exit, And Terms

Use this file when the task asks for valuation, investment return, IC memo, term sheet comments, or deal recommendations.

## 1. Investment Decision Bridge

Every investment recommendation should connect five items:

1. Value: why the company should be worth owning.
2. Valuation: what price is reasonable for that value and risk.
3. Exit: how the fund can turn paper value into cash.
4. Risk: what can break the thesis or delay return.
5. Strategy: why this fund should own this asset now.

If any item is missing, mark it as an open issue. A good company can still be a bad investment if valuation, exit, or terms do not work.

## 2. Choose The Valuation Method

| Situation | Useful methods | Watchouts |
| --- | --- | --- |
| Stable profitable company | P/E, EV/EBITDA, DCF, precedent transactions | normalize earnings, debt-like items, working capital, tax, one-offs |
| High-growth revenue company | EV/Sales, ARR multiple, cohort/unit economics, DCF scenario | revenue quality, churn, gross margin, cash burn |
| Early tech / biotech | milestone valuation, probability-adjusted scenarios, comparable rounds | technical/regulatory probability, funding need, dilution |
| Platform / internet | users, transaction volume, ARPU, LTV/CAC, network value proxy | active vs registered users, monetization, retention |
| Asset-heavy | NAV, replacement cost, DCF from contracted cash flow | title, permits, capex, liabilities, utilization |
| M&A / buyout | normalized EBITDA, DCF, precedent deals, synergies | do not pay for synergy twice; test closing leakage |

Do not pick the method that produces the preferred answer. Explain why the chosen method matches the target's economics.

## 3. Normalize The Base

Before applying any multiple:

- Normalize revenue for returns, rebates, related-party transactions, one-off projects, channel loading, and disputed contracts.
- Normalize EBITDA/net profit for owner compensation, related-party expenses, one-off subsidies, nonrecurring gains/losses, capitalized expenses, bad debt, inventory write-down, and tax adjustments.
- Reconcile profit with operating cash flow and working capital.
- Rebuild gross margin by product/customer/channel where possible.
- Separate historical performance, management forecast, and adjusted diligence forecast.

## 4. Forecast And Return Case

Build at least base/downside/upside cases when materials allow.

Minimum model logic:

- Revenue = volume/users/customers/orders x price/take rate/ARPU.
- Gross profit = revenue x normalized gross margin by segment.
- EBITDA / net profit = gross profit - sales - R&D - G&A - one-off/nonrecurring adjustments.
- Free cash flow = operating profit - tax - working capital increase - maintenance/growth capex.
- Exit value = exit metric x exit multiple, or DCF terminal value.
- Investor proceeds = ownership x exit value plus dividends/minus dilution/transaction costs.

Check:

- Does growth require capex, working capital, licenses, hiring, or customer acquisition spend not in the model?
- Does the fund-life support the exit timing?
- Does downside return rely on optimistic buyback, future financing, or listing assumptions?
- Are multiple expansion and operating growth both assumed without evidence?

## 5. Exit Analysis

Common exit paths:

- IPO: assess listing eligibility, timetable, market window, lock-up, compliance obstacles, and comparable listed companies.
- M&A: assess likely buyers, strategic rationale, regulatory approvals, synergy, and prior transaction evidence.
- Secondary transfer: assess shareholder rights, information availability, market appetite, and valuation discount.
- Repurchase / redemption: assess trigger, obligor capacity, enforceability, dispute cost, and liquidity source.

Rules:

- IPO is not an exit plan by itself; it is a probabilistic path with timing and compliance constraints.
- Repurchase, buyback, and VAM are downside protection or risk allocation, not the base return engine unless the obligor has clear capacity and legal enforceability.
- If there is no credible exit path and no executable redemption, state that the investment may trap capital.

## 6. Translate Risks Into Terms

| Risk / uncertainty | Term response |
| --- | --- |
| Revenue authenticity or collection uncertainty | CP for customer confirmation, special indemnity, escrow, price adjustment |
| Earnings normalization uncertainty | earnout, closing accounts, EBITDA adjustment, audit right |
| Working capital pressure | normalized working capital peg, debt-free/cash-free adjustment, covenants |
| Legal title / equity defect | CP for rectification, founder reps, indemnity, closing condition |
| Related-party dependence | pricing policy, termination/novation plan, board reserved matter, disclosure covenant |
| Governance weakness | board seat, veto rights, information rights, internal-control remediation |
| Founder/key-person risk | founder lock-up, vesting, non-compete, good/bad leaver, retention plan |
| Listing delay | staged investment, valuation adjustment, redemption right, milestone covenant |
| Technology/regulatory milestone | tranche investment, milestone-based valuation, IP reps, expert confirmation |
| Environmental/tax/labor issue | special indemnity, escrow, rectification before closing, specialist opinion |

## 7. Core Term-Sheet Areas

Review at least:

- Securities type, investment amount, pre-money/post-money valuation, ownership, ESOP treatment.
- Use of proceeds, tranches, milestones, and conditions precedent.
- Board composition, observer rights, reserved matters, information rights, inspection/audit rights.
- Transfer restrictions, ROFR, co-sale, drag/tag, founder lock-up.
- Liquidation preference, anti-dilution, redemption/repurchase, VAM/earnout, dividends.
- Founder commitments, non-compete, confidentiality, IP ownership, employment/vesting.
- Reps/warranties, disclosure schedule, indemnity cap/basket/survival, special indemnity, escrow/holdback.
- Closing mechanics, MAC, covenants between signing and closing, post-closing obligations.

## 8. Recommendation Language

Use a conclusion like:

```text
At the current valuation, the deal is investable only if [core uncertainty] is resolved through [evidence] and [term protection]. Without this, the return case depends on [unsupported assumption], so the recommendation is [pause / reprice / conditionally proceed].
```

Avoid:

- "The company is good, so valuation is acceptable" without return math.
- "IPO exit is expected" without eligibility, timeline, and lock-up analysis.
- "Founder buyback protects downside" without capacity and enforceability analysis.
