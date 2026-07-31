---
name: private-equity-investment-dd
description: "把 BP/CIM、访谈纪要、数据室和财务法律材料转成证据驱动的私募股权尽调与 IC 决策包。Use for PE/VC, growth equity, buyout, M&A, strategic investment, Pre-IPO, or non-listed-company diligence, including evidence matrices, red flags, QoE, valuation/return cases, terms, management interviews, data requests, IC memos, and post-investment value creation."
---

# Private Equity Investment DD

Use this skill to turn messy investment materials into a professional internal due diligence report or IC memo. The skill is derived from Noah's local DD book pack and is for internal investment research, not public investment advice.

## 中文介绍

这个 Skill 把零散的 BP、CIM、访谈、财务表、合同和数据室文件，组织成一套能支持投委会判断的尽调证据系统，而不是简单复述管理层故事。

- **适合谁**：PE/VC、并购、战略投资、Pre-IPO 和成长股权团队，以及需要准备 IC 材料的项目负责人。
- **解决什么**：把商业、行业、财务、法律税务、团队、估值、回报、退出和交易条款放进同一套决策逻辑。
- **标准产出**：基础事实包、投资假设、证据矩阵、红旗台账、数据请求清单、管理层访谈提纲、估值回报桥和专业 HTML 尽调报告。
- **核心价值**：每个重要主张都要对应来源、核验状态、证据缺口和交易影响；信息不足时输出缺口驱动报告，不把未知包装成确定性。

For full DD reports, default to a standalone HTML report unless Noah asks for another format. The HTML should be report-ready, evidence-aware, and suitable for internal IC circulation.

## Default Output

Unless Noah asks otherwise, produce:

1. Executive investment judgment: proceed / conditional proceed / pause / reject.
2. Basic information pack: legal entity, aliases, history, shareholders, capital, governance, licenses, products, team, financing, transaction terms, and material-source boundary.
3. Investment thesis and key assumptions.
4. Evidence matrix: claim -> evidence -> source -> verification status -> gap -> deal implication.
5. Integrated business, industry, financial, legal/tax, team, valuation, exit, and post-investment analysis.
6. Red-flag register and next-step data/interview request list.
7. Standalone HTML report using `references/html-report-output.md` and `references/report-structure.md` for full DD; use Markdown only for quick scans or when requested.

## Operating Contract

1. Classify the deal first: growth equity, buyout, M&A, strategic investment, Pre-IPO, VC, minority investment, or unknown.
2. Identify the decision stage: screening, preliminary DD, full DD, IC, term-sheet negotiation, or post-DD remediation.
3. Select the relevant deal/stage adapter from `references/special-dd-adapters.md` and industry adapter from `references/industry-dd-adapters.md`. If no adapter fits, use the general full-scope checklist and state the assumption.
4. Inventory supplied materials by type: BP/CIM, financials, contracts, data room, interview notes, meeting minutes, public information, third-party reports.
5. Run the basic-information extraction protocol in `references/basic-information-extraction.md` before writing analytical sections. A DD report must not skip factual company and transaction information just because the investment conclusion is clear.
6. Apply the book-fusion coverage rules in `references/book-fusion-coverage.md`: every full report should combine the five source-book lenses instead of relying on only one checklist style.
7. Build an initial investment thesis before summarizing materials. Ask what must be true for the deal to work.
8. Convert all major claims into an evidence matrix. Never let management claims sit as conclusions.
9. Cross-check business, financial, and industry evidence:
   - business DD asks what the company actually does;
   - financial DD quantifies and tests whether the business story is true;
   - industry DD benchmarks whether the story is attractive and defensible.
10. Build valuation, return, exit, and terms analysis using `references/valuation-and-terms.md`.
11. Run red-flag gates before writing a positive recommendation. Use `references/red-flag-playbook.md` and `references/evidence-and-red-flags.md`.
12. Draft the report conclusion-first. Separate facts, calculations, interpretations, management claims, and evidence gaps.
13. For full DD output, generate standalone HTML and verify it locally: parseable HTML, responsive layout, no page-level horizontal overflow, and no exposed private IDs/tokens/raw sensitive content.
14. End with deal implications: valuation adjustment, conditions precedent, reps/warranties, covenants, closing conditions, post-investment actions, or reasons to stop.

## Source Book Pack

Read `references/source-books.md` when you need the provenance of the framework or want to cite which local book contributed a method.

Core synthesis:

- Ding Min: PE investment first principles, decision mechanism, DD report elements, valuation, negotiation, and deal terms.
- Qi Wei: investment logic, business-finance-industry triangulation, growth verification, investment memo/report structure.
- Zhou Tao: financial DD logic, on-site work, interviews, third-party validation, nonfinancial-to-financial cross-checks, QoE-style report writing.
- Hui Zengqiang / Lu Na: comprehensive financial, legal, business, special-type DD procedures and report templates.
- Guoming/Sun Peiyuan white paper: concise process, methods, and classic checklist coverage.

## When Writing A Report

Use these references as needed:

- `references/report-structure.md`: full investment DD report and IC memo structure.
- `references/workflow.md`: step-by-step execution flow from raw materials to final report.
- `references/basic-information-extraction.md`: mandatory factual extraction tables for company basics, transaction facts, material inventory, and source conflicts.
- `references/book-fusion-coverage.md`: module-by-module map showing how the five local DD books should be fused in each report.
- `references/html-report-output.md`: standalone HTML report requirements, layout guidance, sensitive-content rules, and browser QA checklist.
- `references/module-checklists.md`: detailed module-by-module analysis and verification checklist. Use this for full DD reports, IC memos, and any request where Noah asks for professional depth.
- `references/special-dd-adapters.md`: stage and transaction-type adapters for VC/growth, Pre-IPO, buyout/M&A, strategic investment, asset-heavy, factoring/supply-chain, real estate/infrastructure/mining/overseas, and similar special cases.
- `references/industry-dd-adapters.md`: industry-specific diligence lenses for hard tech, semiconductor, pharma/medical, SaaS/platform, manufacturing, consumer/channel, project engineering, and asset-heavy models.
- `references/valuation-and-terms.md`: valuation method selection, return bridge, exit feasibility, and term-sheet protection logic.
- `references/evidence-and-red-flags.md`: evidence hierarchy, red-flag gates, and verification rules.
- `references/red-flag-playbook.md`: module-level red-flag cards with triggers, checks, and deal actions.
- `references/interview-and-data-room.md`: data request lists and interview guides.
- `references/report-writing-examples.md`: report-writing patterns, conclusion language, risk phrasing, assumptions, and IC memo compression.
- `references/self-test.md`: prompts to test whether the skill behaves correctly.

## Quality Rules

- Do not invent missing financials, customers, contracts, litigation, or valuation assumptions.
- Mark each important item as confirmed fact, calculated fact, management claim, third-party evidence, interpretation, or open question.
- Treat legal, tax, environmental, IP, labor, litigation, and regulatory issues as specialist-verification areas. State the risk and required professional follow-up; do not give final legal opinions.
- For sensitive private materials, summarize and synthesize. Do not expose raw contracts, private IDs, bank details, personal information, or confidential transaction terms in user-facing replies.
- If source materials are insufficient, produce a gap-driven report and a prioritized data request list rather than pretending the DD is complete.
- For each report module, use the detailed checklist in `module-checklists.md`; do not stop at a high-level heading if the source materials contain enough detail to verify deeper sub-items.
- For basic company information, do not compress away factual tables. Include the facts, source status, conflicts, and follow-up action even when the company is early-stage or materials are incomplete.
- If the company is early-stage, industry-specific, asset-heavy, Pre-IPO, or transaction-structured, adapt the checklist. Do not force the same financial/legal emphasis onto every deal.
- Treat buyback, valuation adjustment, and VAM/earnout mechanisms as downside protection or risk allocation unless the evidence shows they are executable exit paths.
- For HTML reports, never include raw sensitive identifiers, private personal data, credentials, Feishu internal IDs, API tokens, bank account details, or unredacted contract signatures in user-facing output. Summarize or redact instead.

## Self-Check Before Final

Before delivering, verify:

- The basic-information section covers the target entity, transaction, materials reviewed, cap table/governance, products, team, and source conflicts.
- The investment conclusion is traceable to evidence.
- The five-book fusion lens has been applied: PE decision/terms, investment logic, financial/QoE, comprehensive legal/business DD, and classic checklist/process discipline.
- Growth, margin, cash flow, valuation, and exit assumptions are internally consistent.
- Management projections have been challenged and revised where evidence requires it.
- Red flags have deal implications, not just descriptions.
- The report says what to do next: proceed, pause, reject, reprice, renegotiate, request data, or escalate to specialists.
- Full HTML reports have passed basic local validation: parseable HTML, readable on desktop/mobile, tables scroll or fit, and sensitive scan is clean.
