# Workflow

## 0. Intake

Capture:

- Deal name and company aliases.
- Deal type: growth equity, buyout, M&A, strategic investment, Pre-IPO, VC, minority investment, unknown.
- Decision stage: screening, preliminary DD, full DD, IC, term sheet, closing, post-DD remediation.
- Investment role: financial sponsor, strategic buyer, minority investor, lender-like investor, corporate development.
- Output expected: red-flag scan, full DD report, IC memo, data request list, interview guide, valuation/return case.
- Materials provided and missing.

## 1. Material Inventory

Classify input files and notes:

- Company basics: BP, CIM, website, org chart, cap table, history, shareholder structure.
- Financials: audit reports, management accounts, trial balance, general ledger, revenue/cost details, bank statements, tax filings, budgets, forecasts.
- Business data: customer list, contracts, pipeline, orders, backlog, churn, pricing, unit economics, production/sales/usage data.
- Industry data: market reports, peer data, expert calls, customer/supplier interviews, competitor evidence.
- Legal/tax: licenses, articles, board/shareholder resolutions, contracts, IP, litigation, compliance, labor, environmental, related-party records.
- Meetings and interviews: management, finance, sales, production, R&D, HR, customers, suppliers, competitors, bankers, lawyers, accountants.

For full DD, convert the inventory into a source-boundary table using `basic-information-extraction.md`. Do this before writing conclusions so the report shows what is original, draft, meeting-derived, unverified, missing, or conflicting.

## 2. Basic Information Pack

Extract factual material before analysis:

- entity basics and operating status;
- historical milestones;
- ownership, cap table, paid-in status, governance, ESOP;
- transaction facts, term-sheet evolution, closing conditions;
- products/SKUs/roadmap and actual stage;
- team and organization basics;
- finance basics: revenue status, cash, burn, debt, related-party balances, forecasts;
- source conflicts and missing attachments.

Use signed/original documents over term sheets, drafts, AI summaries, and management interviews. If facts conflict, keep the conflict visible and state the evidence hierarchy.

## 3. Investment Thesis

Write the deal thesis before summarizing details:

- What is the asset?
- Why now?
- What must be true for the investment to work?
- What is the expected source of return: growth, margin expansion, multiple expansion, deleveraging, cash yield, consolidation, synergy, turnaround, exit optionality?
- Which assumptions most affect downside?

## 4. Adapter Selection

Before expanding the analysis, select:

- transaction/stage adapter from `special-dd-adapters.md`;
- industry/economic-engine adapter from `industry-dd-adapters.md`;
- valuation and terms lens from `valuation-and-terms.md`.

Record the selected adapters in the report or working notes. If the deal combines multiple types, use multiple adapters, but explain which one drives the investment decision. Example: a Pre-IPO semiconductor company should use both the Pre-IPO adapter and the semiconductor adapter.

## 5. Book Fusion Coverage

Apply `book-fusion-coverage.md` for full reports:

- Ding Min: investment decision, valuation, negotiation, terms.
- Qi Wei: investment logic, business-finance-industry triangulation, value/valuation/exit/risk.
- Zhou Tao: financial DD, order-revenue-collection, on-site and nonfinancial cross-check.
- Hui/Lu: comprehensive business/financial/legal/tax DD taxonomy.
- Guoming/Sun Peiyuan: classic process, company history, assets, HR, contract, litigation, environmental, IP checklist.

If a module is thin, state whether the source materials are missing or the module is not relevant to the deal.

## 6. Hypothesis Tree

Break the thesis into testable questions:

| Workstream | Core question |
| --- | --- |
| Business model | What does the company sell, to whom, how, and why does the customer buy? |
| Product/technology | Is the product real, differentiated, scalable, and defensible? |
| Customers/revenue | Are revenue, orders, backlog, retention, pricing, and customer concentration healthy? |
| Market/industry | Is the market large, growing, accessible, and attractive under realistic segmentation? |
| Competition | Is the company advantaged versus peers on product, cost, channel, brand, data, license, or execution? |
| Financial quality | Are revenue, margin, EBITDA, working capital, capex, tax, and cash conversion credible? |
| Management/team | Is the team competent, honest, aligned, and able to execute the plan? |
| Legal/tax/compliance | Are there deal-blocking or price-changing legal, tax, labor, environmental, IP, regulatory, contract, or litigation risks? |
| Valuation/return | Does the price work under revised projections and realistic exit assumptions? |
| Post-investment | What must be done after closing to protect and create value? |

For a full report, expand each workstream using `module-checklists.md` before drafting. Then add the selected deal and industry adapter checks. The hypothesis tree is only the top layer; the detailed checklist prevents the agent from skipping product, order, cash, legal, contract, IP, HR, environmental, and report-review checks.

## 7. Evidence Matrix

For every important claim, build:

| Claim | Evidence | Source | Status | Gap | Deal implication |
| --- | --- | --- | --- | --- | --- |

Statuses:

- confirmed fact
- calculated fact
- management claim
- third-party evidence
- interpretation
- unresolved conflict
- open question

## 8. Triangulation

Run these cross-checks:

- Product claim -> contracts/SKUs/demo/customer feedback/revenue mix.
- Revenue growth -> orders/backlog/invoices/acceptance documents/collections/customer interviews.
- Margin claim -> product mix/pricing/procurement/labor/production yield/peer margin.
- Market size -> bottom-up customer count and spend, not only broad market reports.
- Customer quality -> concentration, repeat purchase, churn, satisfaction, payment behavior, switching cost.
- Management forecast -> historical delivery, pipeline conversion, capacity, hiring, capex, working capital, funding.
- Valuation -> revised forecast, comparable companies/transactions, exit path, dilution, terms, downside case.

Also run module-level triangulation:

- Industry boundary -> actual customer segment -> product scope -> comparable companies.
- Product claim -> SKU/contract/demo/IP/R&D payroll/procurement evidence.
- Core capability -> customer reason to buy -> margin/retention/cash conversion.
- Legal asset/title -> business necessity -> valuation/closing implication.
- Founder/team claim -> employee/customer/supplier/lender feedback.

## 9. Valuation, Exit, And Terms Bridge

Use `valuation-and-terms.md` before drafting the recommendation:

- select a valuation method that matches the target's economics;
- normalize the financial base before applying multiples;
- test base/downside/upside return cases;
- evaluate exit path feasibility and fund-life fit;
- translate unresolved risks into price, CPs, reps/warranties, indemnity, escrow, governance, covenants, tranches, or rejection.

Do not allow a positive business narrative to bypass valuation and exit discipline.

## 10. Red-Flag Gate

Before writing a positive conclusion, apply `evidence-and-red-flags.md` and `red-flag-playbook.md`.

Classify red flags:

- P0: potential deal-stopper or must-escalate.
- P1: price/terms/condition precedent issue.
- P2: monitor or post-investment action.

## 11. Report Draft

Use `report-structure.md`, `html-report-output.md`, and `report-writing-examples.md`. Write conclusion-first:

1. Recommendation.
2. Why the deal could work.
3. What the evidence supports.
4. What remains unverified.
5. What changes price, terms, or process.

For full DD, generate standalone HTML unless another format is requested. The HTML report must include both the investment analysis and the factual DD tables, especially company basics, cap table/governance, transaction facts, source conflicts, and data gaps.

## 12. Final QA

Check:

- Does the report answer the investor's decision, not just summarize the company?
- Does it include enough basic information for an IC reader to understand the target and transaction without opening raw files?
- Are all key assumptions evidenced or marked as gaps?
- Has the five-book fusion lens been applied across modules?
- Are the risk implications explicit?
- Is the next action clear?
- If HTML was generated, did it pass parser, sensitive-content, desktop, and mobile checks?
