# Investment Due Diligence Report Structure

Use this as the default full report. For IC memo, compress sections but keep the same logic. For the actual analysis required inside each section, also read `module-checklists.md`; this file defines the report spine, while `module-checklists.md` defines the verification depth. For full HTML reports, also read `html-report-output.md`. For factual extraction, read `basic-information-extraction.md`. For stage-specific, industry-specific, valuation, red-flag, and phrasing guidance, use `special-dd-adapters.md`, `industry-dd-adapters.md`, `valuation-and-terms.md`, `red-flag-playbook.md`, and `report-writing-examples.md`.

## Cover

- Project name.
- Target company.
- Deal type and stage.
- Date.
- Prepared for internal investment review.
- Confidentiality note.

## 0. Executive Judgment

Start with:

- Recommendation: proceed / conditional proceed / pause / reject.
- One-sentence investment thesis.
- Proposed investment amount, valuation, ownership, and instrument if available.
- Top 3 upside drivers.
- Top 3 risks or unresolved evidence gaps.
- Required next actions before IC or signing.

## 1. Deal Context

- Transaction background.
- Seller/founder fundraising objective.
- Investor role and strategic/financial purpose.
- Timeline, process, exclusivity, advisors, and constraints.
- Materials reviewed and missing materials.
- Source hierarchy and conflicts: signed/original vs draft/term sheet vs meeting note vs management claim.

## 2. Basic Information And Evidence Boundary

This section is mandatory for full DD reports. Use tables, not only paragraphs.

- Material boundary:
  - files and cloud documents reviewed;
  - source type, version/date, purpose, evidence status, limitation.
- Entity basics:
  - legal name, aliases, brand names;
  - legal representative, establishment date, operating status, address if appropriate;
  - registered capital, paid-in capital, operating term, business scope, actual business;
  - subsidiaries/branches/platforms/investees/offshore structures;
  - licenses, permits, certifications, filings;
  - sensitive identifiers redacted from user-facing output.
- History and milestones:
  - formation, restructurings, financing rounds, product milestones, IP transfers, major contracts, regulatory events.
- Ownership and governance:
  - pre/post cap table;
  - capital contribution deadlines/status;
  - controller and beneficial ownership;
  - shareholder platforms/ESOP;
  - board/director/supervisor/observer/reserved matters.
- Transaction facts:
  - amount, valuation, ownership, instrument, prior term-sheet evolution, closing conditions, use of proceeds, investor rights.
- Basic product/team/finance:
  - product lines and stage;
  - team/org facts;
  - revenue status, cash, burn, debt, budget, financing runway where available.

## 3. Investment Thesis And Assumption Map

- Core thesis.
- Selected transaction/stage adapter.
- Selected industry/economic-engine adapter.
- Selected source-book lenses from `book-fusion-coverage.md`.
- What must be true.
- Assumption table:

| Assumption | Why it matters | Evidence | Status | Falsification test | Deal implication |
| --- | --- | --- | --- | --- | --- |

## 4. Company Overview

- History and milestones.
- Ownership and cap table.
- Organization and governance.
- Products/services.
- Business model.
- Revenue model and cost structure.
- Key assets, licenses, IP, facilities, and operating footprint.

## 5. Market And Industry DD

- Market definition and segmentation.
- Market size using top-down and bottom-up checks.
- Growth drivers and constraints.
- Industry value chain and profit pools.
- Competitive landscape.
- Regulation and technology trends.
- Customer adoption logic.
- Judgment: attractive / mixed / unattractive, with evidence gaps.

Minimum checks: industry boundary, industry logic, development history, current state, trend, value chain, competitive landscape, major market participants, customer budget and actual reachable market. Do not use a broad market size if the target only serves a narrow segment.

## 6. Business And Commercial DD

- Product/service truth: what is actually sold and delivered.
- Customer profile, use case, purchasing process, and budget owner.
- Revenue composition by product, customer, region, channel, and contract type.
- Sales pipeline, orders, backlog, conversion, churn, retention, and repeat purchase.
- Pricing power and discounting.
- Customer concentration and dependence.
- Supplier/channel dependence.
- Unit economics and scalability.
- Core capability: product capability, transaction/channel capability, supply-chain/operation capability, regulatory/license capability, data/platform capability, or service execution capability.
- Judgment: what is proven, what is only claimed, and what must be verified next.

Minimum checks: product system, product definition, product function/structure/working principle, use cases, technology principle, core technical indicators, R&D/IP position, commercial model, core capability, customer/supplier/channel dependence.

## 7. Financial DD / Quality Of Earnings

- Historical financial summary.
- Revenue quality:
  - revenue recognition;
  - order/invoice/acceptance/collection bridge;
  - recurring vs one-off;
  - customer concentration;
  - related-party or channel stuffing risk.
- Gross margin and profitability:
  - product/customer/channel mix;
  - pricing and cost drivers;
  - peer comparison;
  - abnormal margin test.
- EBITDA adjustments:
  - one-off income/cost;
  - owner-related expenses;
  - nonrecurring subsidies;
  - capitalization policies;
  - normalization adjustments.
- Working capital:
  - receivables aging and collections;
  - inventory quality and turnover;
  - payables and supplier terms;
  - deposits/prepayments/deferred revenue.
- Cash flow:
  - OCF vs EBITDA;
  - free cash flow;
  - capex requirements;
  - financing need.
- Tax and internal control:
  - tax compliance;
  - invoice practices;
  - cash transactions;
  - related-party payments;
  - accounting policy consistency.
- Forecast review:
  - management forecast;
  - revised forecast;
  - key sensitivities.

Minimum checks: revenue/order/collection bridge, nonfinancial data cross-checks, working capital, tax, internal control, related parties, cash conversion, management forecast revision, and valuation impact.

## 8. Legal, Tax, Compliance, And Transaction Risk

State that specialist verification is required for final opinions.

Cover:

- Subject qualification and valid existence.
- Shareholder qualification, capital contribution, equity history, pledge, disputes.
- Corporate governance and authorization.
- Major assets and title.
- IP ownership, licensing, infringement, renewal, and control-change risk.
- Major contracts, change-of-control clauses, exclusivity, termination, penalties.
- Debt, guarantees, pledges, off-balance-sheet commitments.
- Related-party transactions and tunneling.
- Labor, social insurance, employee disputes, non-compete.
- Tax compliance and incentives.
- Environmental, safety, quality, and regulatory permits.
- Litigation, arbitration, administrative penalties, investigations.
- Closing deliverables, conditions precedent, reps/warranties, indemnities, covenants.

Minimum checks: subject qualification, historical equity changes, capital contribution, asset title, IP validity, major contract transferability/termination/liability, debt/guarantees, related parties, tax, labor, environmental/safety/quality, litigation/penalties, approvals required for the transaction.

## 9. Management And Organization

- Founder/management background.
- Strategic judgment and execution record.
- Integrity and transparency.
- Incentive alignment.
- Key-person risk.
- Organization capability and talent gaps.
- Management forecast credibility.
- Interview inconsistencies and follow-up questions.

Minimum checks: founder integrity, strategy capability, execution capability, organization depth, key-person risk, employee incentives, ordinary employee feedback, management turnover, external reputation, and alignment with the deal terms.

## 10. Valuation, Return, And Exit

- Proposed valuation and instrument.
- Valuation method fit: revenue multiple, EBITDA multiple, DCF, comparable transactions, net asset value, milestone/scenario model, or industry-specific method.
- Revised base/upside/downside cases.
- IRR/MOIC table and key assumptions.
- Sensitivity: growth, margin, working capital, capex, exit multiple, timing, dilution.
- Exit path: IPO, strategic sale, sponsor-to-sponsor, buyback, dividend recap, secondary transfer.
- Deal terms needed to protect downside.

Minimum checks: value/valuation/exit/risk coherence, revised forecast, investment and exit multiples, IRR/MOIC, dilution, timing, downside case, fund-life fit, buyback/redemption executability, and terms required to protect against unverified assumptions.

## 11. Red Flags And Deal Implications

| Severity | Issue | Evidence | Impact | Required action |
| --- | --- | --- | --- | --- |

Translate every serious issue into:

- stop;
- reprice;
- condition precedent;
- escrow/holdback;
- reps and warranties;
- indemnity;
- covenant;
- specialist review;
- post-investment action.

## 12. Post-Investment Value Creation

- First 100 days.
- Finance/accounting normalization.
- Sales/customer expansion.
- Pricing and product mix.
- Cost and working capital improvement.
- Governance and reporting.
- Talent and incentive plan.
- Exit-readiness or IPO-readiness.

## 13. Appendices

- Materials reviewed.
- Interview list.
- Data request list and status.
- Evidence matrix.
- Financial model assumptions.
- Specialist report summaries.
- Open questions.

## HTML Report Compression

When producing a full HTML report, keep the same logic but use an IC-readable sequence:

1. Cover/hero.
2. Table of contents.
3. Executive judgment.
4. Material and evidence boundary.
5. Basic information and history.
6. Equity, governance, transaction facts.
7. Team and organization.
8. Market and competition.
9. Product, technology, business model.
10. Customers/revenue/operations.
11. Financial, tax, valuation.
12. Legal/compliance/transaction terms.
13. Red flags, data gaps, closing conditions, post-investment plan.
14. Final recommendation and decision scenarios.

## IC Memo Compression

For a short IC memo, use:

1. Executive recommendation.
2. Deal terms.
3. Investment thesis.
4. Key evidence.
5. Major risks and mitigants.
6. Valuation/return.
7. Open items and decision request.
