# Module Checklists

Use this file when writing a full investment DD report, IC memo, red-flag scan, or professional project review. It expands each report module into specific analysis and verification steps distilled from the five source books.

Do not mechanically include every bullet in the final report. Use the checklist to inspect materials, identify gaps, and decide what belongs in the report.

## Coverage Audit

Current v1 gap before this reference was added:

| Module | Prior depth | Required upgrade |
| --- | --- | --- |
| Intake and process | Adequate | Add decision-stage, role, timeline, work plan, bottom-paper discipline. |
| Industry | Too high-level | Add industry boundary, logic, history, current state, trend, chain, competition, participants. |
| Business/product | Too high-level | Add product system, product definition, function/structure/principle, applications, technology indicators, core capability. |
| Customer/revenue | Partial | Add order-revenue-collection bridge, customer quality, renewal/churn, contract terms, related-party customer risk. |
| Financial/QoE | Good spine, not enough checks | Add nonfinancial cross-checks, walkthrough tests, forecast revision, tax/internal control, cash conversion. |
| Legal/compliance | Good categories, not enough tests | Add subject qualification, equity history, asset title, IP validity, major-contract review, labor/environment/litigation. |
| Management/team | Too brief | Add founder integrity, ordinary employees, incentive, organization depth, management changes, external reputation. |
| Valuation/return/exit | Adequate | Add value/valuation/exit/risk coherence and valuation adjustment triggers. |
| Report QA | Partial | Add report scope, limitations, assumptions, internal review, appendix/bottom-paper consistency. |

## 0. Process And Work Plan

Source emphasis: Guoming/Sun Peiyuan white paper, Hui/Lu comprehensive guide, Zhou Tao financial DD.

Check:

- Has the project been formally classified by stage: screening, preliminary DD, full DD, IC, signing, closing, post-DD remediation?
- Is the purpose explicit: discover value, identify fatal flaws, support valuation/terms, prepare post-investment actions?
- Has the team defined workstreams: business, financial, legal/tax, industry, management, valuation, specialist?
- Has the team set the data-room request list, interview plan, on-site plan, external validation plan, and review cadence?
- Are materials numbered or indexed so the final report can trace conclusions back to bottom papers?
- Are assumptions, date cutoffs, report scope, reliance on third-party reports, and limitations stated?
- Is there a daily or periodic issue log: issue, owner, evidence, needed follow-up, deadline, deal impact?

Minimum output:

- Work plan summary.
- Materials received/missing table.
- Interview and verification plan.
- Scope and limitation note.

## 1. Company Basics And Legal Existence

Source emphasis: Hui/Lu comprehensive guide, Guoming/Sun Peiyuan white paper.

Check:

- Legal name, aliases, unified social credit code or equivalent, registered address, operating address, legal representative.
- Business license, articles, current and historical amendments, annual filings, operating term.
- Registered capital, paid-in capital, capital contribution method, noncash contribution valuation/title evidence.
- Historical equity changes, share transfers, capital increases, restructurings, mergers, spin-offs, major asset transfers.
- Current shareholders, ultimate beneficial owner, controller, concert parties, employee shareholding platforms, ESOP.
- Equity pledge, freezing, disputes, nominee holding, repurchase obligation, special rights.
- Required licenses, permits, approvals, qualifications, industry access, and whether the business operates within approved scope.
- Subsidiaries, branches, investees, offshore entities, VIE-like or nominee arrangements if any.

For full reports, this module must be visibly present even when evidence is incomplete. Use `basic-information-extraction.md` to create:

- entity basics table;
- history/milestone table;
- ownership/governance/incentive table;
- transaction facts table;
- source conflict and follow-up table.

Report judgment:

- Is the entity validly existing and able to sign/close the contemplated transaction?
- Are equity ownership and control rights clear enough for investment?
- Which historical issues require legal cleanup or condition precedent?

Minimum output:

- Do not hide basic facts in prose. If a fact is unknown, write "not provided" or "requires verification" and add the next evidence request.
- If signed agreements, term sheets, meeting minutes, and management claims disagree, show the conflict and rank evidence quality.

## 2. Industry And Market DD

Source emphasis: Qi Wei investment logic, Ding Min PE handbook, Hui/Lu business DD.

Check:

- Industry boundary:
  - Define by customer need and substitutable product/service, not by broad regulatory industry code or BP wording.
  - Show the industry coordinate system: broad industry -> sub-sector -> target segment -> actual served market.
- Industry logic:
  - What problem does the industry solve?
  - What historical constraint created the opportunity?
  - What changed now: policy, technology, cost curve, customer behavior, supply chain, capital cycle?
- Development history:
  - Stages, inflection points, adoption barriers, regulation, technology shifts, business-model shifts.
- Current state:
  - Market size, growth, penetration, supply/demand, profitability, customer budget, procurement process.
- Future trend:
  - Drivers, constraints, adoption pace, price trend, margin trend, likely consolidation.
- Value chain:
  - Upstream, midstream, downstream, distributors/channels, end customers, profit pools, bargaining power.
- Competitive landscape:
  - Direct competitors, substitutes, incumbents, new entrants, customer self-build, imported/local alternatives.
  - Compare by product performance, price, delivery, service, brand, channel, license, cost, data, customer access.
- Major participants:
  - List target and peers with revenue scale, product position, customer base, funding, market share if available.
- Market-size validation:
  - Run top-down and bottom-up checks.
  - Convert broad TAM into realistic SAM/SOM based on target segment, customer budget, product readiness, channel reach.

Red flags:

- Market definition follows BP or prospectus language but does not identify real customers or competitors.
- Target claims a large market but current products only reach a narrow or low-budget segment.
- Market growth relies on policy slogans without customer adoption evidence.
- Competition is described only as "fragmented" or "blue ocean" without peer data.

## 3. Product, Technology, And Business Model

Source emphasis: Qi Wei business DD, Hui/Lu business DD, Ding Min industry/business framework.

Check:

- Product system:
  - Product families, SKUs, services, modules, hardware/software mix, standard vs customized offerings.
  - Relationship between products: core, auxiliary, bundled, legacy, future roadmap.
- Product definition:
  - Explain what the product is in plain language.
  - Define technical terms and acronyms if IC readers may not understand them.
- Product function, structure, and working principle:
  - What job does it do for customers?
  - What are the main components?
  - How does it work operationally?
  - What part is proprietary versus purchased, integrated, outsourced, open-source, or agency/resale?
- Application cases:
  - Customer, scenario, problem, deployment process, measurable result, renewal/expansion.
  - For customized solutions, show at least one real project flow from demand to delivery and acceptance.
- Technology:
  - Technical principle, core indicators, performance benchmarks, maturity, reliability, production/service constraints.
  - R&D team, roadmap, R&D spend, patents, software copyrights, standards participation, trade secrets.
  - IP ownership and whether key technology depends on founders, third parties, licenses, or former employers.
- Business model:
  - Customer, value proposition, pricing, contract type, sales cycle, delivery, acceptance, renewal, after-sales.
  - Direct sales, distributors, agents, OEM/ODM, project-based, subscription, usage-based, license, service, platform.
- Core capability:
  - Product capability: R&D, patents, performance, productization.
  - Transaction capability: customer access, channel, brand, salesforce, ecosystem, procurement relationships.
  - Operation/supply-chain capability: delivery, cost, quality, working capital, execution.
  - License/regulatory capability: qualification, scarce access, compliance.
  - Data/platform capability: network effects, usage data, switching costs.

Verification:

- Match product claims to contracts, SKU list, demos, technical documents, customer cases, revenue mix, employee skills.
- Compare target's claimed differentiation with customer feedback and competitor benchmarks.
- If the company claims self-developed products, check procurement, source code/IP evidence, R&D payroll, patents, and delivery records.

Red flags:

- Product matrix is confusing and cannot be tied to revenue.
- "Core technology" is mostly integration, agency, or outsourced development but is reported as proprietary.
- Technical indicators are listed without customer value or benchmark.
- Customized projects are presented as scalable standardized products without evidence.

## 4. Customers, Revenue, Orders, And Growth Quality

Source emphasis: Qi Wei, Zhou Tao.

Core principle:

- Order growth is the business signal.
- Revenue growth is the accounting result.
- Collection growth is the cash and customer-quality test.

Check:

- Revenue breakdown by product, customer, channel, region, contract type, project, recurring/nonrecurring.
- Top customer concentration, history, contract duration, pricing, gross margin, receivables, collection, renewal, churn.
- Customer acquisition: source, sales cycle, bid/tender, channel, repeat purchase, referral, paid sales, partner.
- Sales contracts/orders:
  - order source, order date, product details, amount, delivery terms, acceptance criteria, cancellation/return terms.
  - backlog and conversion to revenue.
- Delivery and acceptance:
  - shipment/service record, acceptance document, implementation milestone, customer confirmation, after-sales issue.
- Collection:
  - payment terms, actual collection, overdue amount, aging, disputes, returns, credit notes, third-party payments.
- Customer quality:
  - real use case, satisfaction, budget continuity, switching cost, procurement dependency, strategic importance.
- Growth models:
  - ideal: orders, revenue, and collections rise together.
  - working-capital pressure: orders/revenue rise faster than collections.
  - delivery bottleneck: orders rise but revenue/collection lag.
  - historical backlog consumption: revenue/collection rise while new orders slow.
  - low-quality growth: related-party/channel orders, aggressive discounts, long receivables, return risk.

Verification:

- Build order -> delivery/acceptance -> invoice -> revenue -> receivable -> collection bridges for top customers and sample transactions.
- Compare CRM/pipeline, order ledger, invoices, bank receipts, ERP, tax invoices, and customer confirmations.
- Interview customers to verify use, satisfaction, renewal, alternatives, budget, payment, and switching cost.

Red flags:

- Revenue grows without corresponding orders.
- Orders grow but product details do not match the company's claimed core product.
- Collections lag materially with no credible customer or contract explanation.
- Top customers are related parties, former employees, shareholder-linked entities, or distributor stockpiling.
- Customer concentration is high and renewal is uncertain.

## 5. Sales, Channel, Supply Chain, Production, And Operations

Source emphasis: Hui/Lu business DD, Zhou Tao on-site work, Qi Wei business model sections.

Check:

- Sales model:
  - direct sales, channel, distributor, agency, online, bidding, project sales, key-account sales.
  - sales team size, productivity, incentive, pipeline discipline, discount authority.
- Channel/distributor:
  - buy-sell or agency, inventory policy, rebate, return rights, credit terms, end-customer visibility.
  - channel stuffing, related-party channel, dependence on key distributors.
- Procurement:
  - top suppliers, supply concentration, alternative suppliers, price volatility, credit terms, dependency, exclusivity.
- Production/service process:
  - process flow, bottleneck, capacity, utilization, yield, quality, safety, outsourcing, subcontracting.
- Inventory:
  - raw material, WIP, finished goods, slow-moving, obsolete, consignment, third-party warehouses.
- Quality and after-sales:
  - defect rate, returns, warranty, complaints, product liability, service SLA.
- On-site observations:
  - production-line saturation, equipment condition, employee morale, warehouse state, safety/environmental issues, posted procedures, actual internal-control execution.

Verification:

- Perform walkthrough tests from purchase to production to sales to collection.
- For manufacturing: reconcile capacity, production, sales, inventory, energy use, labor hours, packaging, logistics.
- For project/service companies: reconcile project milestones, labor deployment, subcontractors, acceptance, billing, collection.
- Visit or interview suppliers, customers, and if useful competitors.

Red flags:

- Claimed capacity does not match equipment, staff, bottleneck process, or supplier capacity.
- Sales growth relies on distributors with poor sell-through visibility.
- Inventory grows faster than sales with slow-moving or obsolete items.
- Gross margin improvement lacks procurement, price, mix, or process explanation.

## 6. Financial DD / Quality Of Earnings

Source emphasis: Zhou Tao financial DD, Hui/Lu financial DD, Qi Wei growth/forecast logic.

Check:

- Financial basis:
  - audited vs unaudited, consolidation scope, accounting standard, management-account adjustments.
  - accounting policy and estimate changes, revenue recognition, capitalization, depreciation/amortization, impairment.
- Revenue quality:
  - recognition policy, cutoff, related-party revenue, channel stuffing, returns, bill-and-hold, acceptance gaps.
  - order/invoice/acceptance/collection bridge.
- Gross margin:
  - margin by product/customer/channel/region.
  - material, labor, outsourcing, freight, warranty, production yield, product mix, price.
  - peer margin and historical trend.
- EBITDA/profit normalization:
  - one-off income/cost, subsidies, owner expenses, nonrecurring consulting/legal costs, share-based compensation.
  - aggressive capitalization, R&D treatment, abnormal other income/expense.
- Working capital:
  - receivables aging, overdue, post-period collections, bad debt.
  - inventory aging, valuation, write-downs, turnover.
  - payables, supplier credit, deposits, prepayments, deferred revenue.
  - normalized working capital peg if transaction is buyout/M&A.
- Cash flow:
  - EBITDA to OCF bridge, OCF to FCF, capex maintenance vs growth, financing need.
  - cash balance vs debt, restricted cash, bank statements, undisclosed borrowings.
- Tax:
  - VAT/invoice, income tax, tax incentives, related-party tax, historical penalties, unpaid taxes.
- Internal control:
  - finance team, ERP/accounting system, approval process, cash controls, third-party payments, manual Excel dependence.
- Forecast:
  - management plan, historical forecast accuracy, order/backlog support, capacity, hiring, capex, working capital.
  - revise forecast based on evidence.

Nonfinancial cross-checks:

- Capacity > production > sales, unless there is a clear reason.
- Production/sales vs energy, packaging, logistics, labor, raw material consumption.
- Revenue vs orders, acceptance, tax invoices, collections.
- Margin vs product mix, material cost, process improvement, pricing.
- Payroll/social insurance vs headcount and delivery capacity.

Red flags:

- Profit grows but operating cash flow is persistently weak.
- Receivables grow much faster than revenue.
- Post-period collections or returns contradict year-end revenue.
- Inventory/procurement does not support sales volume.
- Management forecast ignores capacity, hiring, capex, working capital, or customer budget constraints.

## 7. Legal, Tax, Compliance, And Transaction Risk

Source emphasis: Hui/Lu legal DD, Guoming/Sun Peiyuan white paper.

Check:

- Subject qualification and existence:
  - business license, annual filing, operating term, business scope, required approvals.
- Equity and capital:
  - capital contribution, equity transfers, historical resolutions, shareholder qualifications, pledge/freeze/dispute.
- Governance:
  - articles, board/shareholder rules, approval thresholds, authorization for the transaction.
- Independence and related parties:
  - business, assets, staff, finance, organization independence.
  - related-party list, transactions, pricing, approvals, dependence, potential tunneling.
- Major assets:
  - land, property, equipment, vehicles, leases, construction approvals, mortgages, encumbrances.
- IP:
  - patents, trademarks, copyrights, software, trade secrets, domain names.
  - ownership, validity, renewal/annual fees, pledges, licenses, transfer restrictions, infringement.
  - employee inventions, commissioned development, joint development, former-employer disputes.
- Major contracts:
  - sales, procurement, loans, guarantees, leases, R&D, IP, construction, distribution, employment, strategic cooperation.
  - term, missing clauses, rights/obligations balance, restrictions, breach liability, transferability, termination, approval procedure, dispute forum.
  - change-of-control, exclusivity, non-compete, most-favored-nation, minimum purchase, penalty, indemnity.
- Debt, guarantees, and contingent liabilities:
  - loans, bank facilities, shareholder loans, entrusted loans, guarantees, pledges, off-balance commitments.
- Labor:
  - labor contracts, social insurance/housing fund, overtime, dispatch, contractor use, non-compete, employee disputes.
- Tax:
  - taxes paid, arrears, incentives, transfer pricing, invoices, penalties, tax inspections.
- Environmental/safety/quality:
  - permits, EIA, acceptance, waste/emission treatment, safety production, quality certifications, penalties, required future capex.
- Litigation and penalties:
  - lawsuits, arbitration, enforcement, administrative penalties, investigations, potential claims, product liability.

Report rule:

- Legal/tax/compliance conclusions must be framed as risk identification and required specialist verification unless a lawyer/tax specialist report is supplied.

Red flags:

- Equity/title defects, core license missing, IP ownership unclear, major contract non-transferable, material litigation, environmental penalties, tax arrears, undisclosed guarantees.

## 8. Management, Organization, HR, And Culture

Source emphasis: Ding Min PE handbook, Qi Wei management chapter, Hui/Lu HR/legal content, Zhou Tao interview observations.

Check:

- Founder/controller:
  - background, integrity, reputation, prior ventures, litigation/penalties, capital market behavior, transparency.
  - motivation for financing/selling and alignment with investors.
- Management capability:
  - strategy, execution, sales, product, finance, operations, hiring, crisis handling.
  - track record vs past plans and financing commitments.
- Team structure:
  - key executives, tenure, turnover, succession, role clarity, dependence on founder.
- Incentives:
  - compensation, bonus, equity incentive, vesting, lock-up, non-compete, retention plan.
- HR:
  - headcount by function, age/education/tenure, labor contracts, social insurance, overtime, contractors.
- Culture and ordinary employees:
  - employee morale, informal interviews, whether statements align with management's story.
- Forecast credibility:
  - whether management understands drivers, constraints, cash needs, and downside.

Verification:

- Interview CEO, CFO, sales, R&D/product, operations, HR, middle managers, ordinary employees.
- Compare management statements across interviewees and against data.
- Check external reputation via customers, suppliers, lenders, competitors, and public records.

Red flags:

- Founder dominates all knowledge and controls finance with weak systems.
- Management avoids direct answers, restricts access, or changes explanations.
- High turnover in finance/sales/R&D without explanation.
- Incentives encourage short-term revenue at the expense of cash and quality.

## 9. Valuation, Return, Exit, And Terms

Source emphasis: Ding Min valuation/terms, Qi Wei value-valuation-exit-risk logic, Zhou Tao forecast/valuation.

Check:

- Value:
  - What growth and cash-flow drivers create enterprise value?
  - Which core capability makes growth durable?
- Valuation:
  - method fit: revenue multiple, EBITDA multiple, DCF, comparable company, comparable transaction, asset value, user/network metric.
  - adjust for growth quality, cash conversion, customer concentration, margin sustainability, legal/tax exposure.
- Return:
  - base/upside/downside cases.
  - IRR/MOIC, holding period, dilution, follow-on funding, liquidation preference, debt.
- Exit:
  - IPO, strategic sale, sponsor-to-sponsor, founder/company buyback, secondary transfer, dividends.
  - buyer universe, listing feasibility, exit multiple, timing, blocking risks.
- Terms:
  - valuation adjustment, earnout, redemption/buyback, liquidation preference, anti-dilution, board seat, veto rights.
  - reps/warranties, indemnity, escrow/holdback, closing conditions, information rights, non-compete, founder lock-up.

Red flags:

- Valuation only works if management forecast is accepted without adjustment.
- Exit path is asserted but not operationally feasible.
- High valuation plus weak cash conversion produces downside funding risk.
- Legal/compliance defects cannot be priced or protected by terms.

## 10. Red-Flag Register And Deal Implications

Every serious issue must be written as:

| Severity | Issue | Evidence | Why it matters | Deal implication | Required next step |
| --- | --- | --- | --- | --- | --- |

Translate issues into:

- stop;
- pause pending evidence;
- reprice;
- condition precedent;
- escrow/holdback;
- indemnity;
- reps/warranties;
- covenant;
- specialist review;
- post-investment action.

Do not write generic risk language unless it changes a decision, price, term, or action.

## 11. Report Writing And QA

Source emphasis: Qi Wei investment recommendation writing, Hui/Lu report chapter, Zhou Tao financial report writing, Guoming/Sun Peiyuan review/archive process.

Check before final:

- Does the report lead with decision and thesis rather than company encyclopedia?
- Does the report still include enough company encyclopedia material for IC readers: entity, history, cap table, governance, transaction facts, products, team, finance basics, and evidence boundary?
- Are report sections standardized enough for IC readers to scan?
- Is each investment highlight supported by a later section and evidence?
- Does each risk explain business impact, financial impact, and transaction implication?
- Are facts, calculations, management claims, third-party evidence, interpretations, and open questions separated?
- Does the report include scope, methods, materials reviewed, assumptions, date cutoff, limitations, and reliance on third-party reports?
- Are bottom papers, interview notes, and source files consistent with report statements?
- Have internal contradictions been resolved or marked as unresolved?
- Are missing materials converted into a prioritized data request list?
- Is the final recommendation one of: proceed, conditional proceed, pause, reject, reprice, renegotiate, or specialist escalation?
- If the output is HTML, did it pass the validation checklist in `html-report-output.md`?

Typical report balance:

- Executive summary: short, conclusion-first.
- Industry and business: enough to understand the company and growth assumptions.
- Financial DD: detailed enough to verify quality of earnings and cash conversion.
- Legal/tax/compliance: focused on deal-blocking or price-changing issues.
- Valuation and terms: explicit link to revised assumptions and risks.
- Appendix: evidence matrix, data request status, interviews, financial schedules.

## Source-To-Module Map

| Module | Main source books |
| --- | --- |
| Process/work plan/report review | Guoming/Sun Peiyuan, Hui/Lu, Zhou Tao |
| Industry/market | Qi Wei, Ding Min, Hui/Lu |
| Business/product/technology | Qi Wei, Hui/Lu |
| Customers/revenue/growth | Qi Wei, Zhou Tao |
| Financial/QoE | Zhou Tao, Hui/Lu, Qi Wei |
| Legal/tax/compliance | Hui/Lu, Guoming/Sun Peiyuan |
| Management/team | Ding Min, Qi Wei, Hui/Lu, Zhou Tao |
| Valuation/exit/terms | Ding Min, Qi Wei, Zhou Tao |
| Report writing | Qi Wei, Hui/Lu, Zhou Tao |
