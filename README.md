# Private Equity Investment Due Diligence Skill

> 中文说明在前，English documentation follows.

一个用于私募股权、VC/PE、并购、战略投资、Pre-IPO、成长股权投资等非上市公司投资场景的专业尽职调查 Skill。它把杂乱的 BP、访谈记录、会议纪要、财务表、合同、数据室资料、飞书/云文档和本地底稿，转化为可用于内部投委会讨论的投资尽调报告、IC Memo、红旗扫描、资料清单和管理层访谈提纲。

本 Skill 的默认完整交付物是 **standalone HTML 尽调报告**，并强制保留基础信息整理、证据边界、资料缺口、红旗登记表和交易影响判断。

## 目录

- [核心定位](#核心定位)
- [适用场景](#适用场景)
- [不适用场景](#不适用场景)
- [能力亮点](#能力亮点)
- [方法来源](#方法来源)
- [工作流](#工作流)
- [默认输出](#默认输出)
- [HTML 报告要求](#html-报告要求)
- [证据与红旗规则](#证据与红旗规则)
- [安装方式](#安装方式)
- [使用示例](#使用示例)
- [仓库结构](#仓库结构)
- [安全与合规边界](#安全与合规边界)
- [维护建议](#维护建议)
- [English Documentation](#english-documentation)

## 核心定位

这个 Skill 不是普通的“报告模板”，而是一个投资尽调执行框架。它要求 Agent 在输出投资观点之前，先完成四件事：

1. **盘点资料边界**：区分原始文件、签署版、草稿、会议纪要、AI 转写、管理层口径、第三方报告和未打开附件。
2. **抽取基础信息**：主体信息、历史沿革、股权结构、治理、激励、交易条款、产品线、团队、财务基础、证据冲突和资料缺口。
3. **建立证据矩阵**：把核心判断拆成 claim -> evidence -> source -> status -> gap -> deal implication。
4. **转化为交易动作**：所有重大问题必须落到继续、暂停、重定价、交割条件、陈述保证、赔偿、托管、治理权、投后动作或放弃交易。

## 适用场景

适合以下任务：

- 私募股权投资尽职调查报告
- VC/成长股权项目初步尽调
- Pre-IPO 项目投资建议书
- 控股收购、并购、少数股权投资、战略投资
- IC Memo / 投委会材料
- 红旗扫描与交易风险判断
- 数据室资料清单和缺口清单
- 管理层、客户、供应商、员工、专家访谈提纲
- 财务尽调 / QoE 初稿
- 估值、回报、退出、交易条款分析
- 投后 100 天计划和价值创造建议

## 不适用场景

以下场景不建议作为主 Skill 使用：

- A 股、港股、美股等上市公司年报财务排雷
- 二级市场股票买卖建议
- 法律意见书、审计报告、税务意见书的替代
- 需要最终专业签字责任的法律、税务、审计、专利、环保、安全生产判断

对于法律、税务、知识产权、劳动、环保、安全、诉讼和监管问题，本 Skill 只做风险识别和资料请求，不给最终专业意见。

## 能力亮点

### 1. 基础信息不会被省略

完整报告必须包含：

- 材料边界和证据状态
- 公司名称、别名、法定代表人、成立时间、经营状态、注册资本、实缴资本
- 历史沿革和重大里程碑
- 投前/投后股权结构
- 控制权、治理、董事/监事/观察员、重大事项保护
- 股权激励、员工持股平台、出资安排
- 交易金额、估值、持股、工具、交割条件、资金用途
- 产品线、产品阶段、商业化进展
- 团队结构、关键人员、能力缺口
- 财务基础、现金、burn rate、收入状态、融资历史
- 源文件冲突和待补资料

### 2. 五本尽调书逐模块融合

Skill 不是只套用一个 checklist，而是把五类方法合在一起：

| 方法视角 | 作用 |
| --- | --- |
| PE 决策与交易条款 | 判断能不能投、怎么定价、怎么保护下行风险 |
| 投资逻辑三角验证 | 行业、业务、财务相互校验 |
| 财务尽调 / QoE | 订单、收入、回款、现金流、营运资金、预测挑战 |
| 全流程业务/法律/财务 DD | 主体、股权、合同、资产、IP、劳动、税务、合规 |
| 经典底稿与清单纪律 | 材料边界、访谈、底稿、附件、复核和归档 |

### 3. 默认输出 HTML 报告

完整报告默认生成 standalone HTML，便于本地打开、投委会阅读、后续转 PDF 或归档。

HTML 报告会强调：

- 结论先行
- 表格化事实整理
- 证据状态标记
- 红旗和交易动作
- 移动端/桌面端可读
- 敏感信息不外露

### 4. 以交易影响为终点

每个红旗必须回答：

- 是否停止交易？
- 是否暂停等待证据？
- 是否需要重定价？
- 是否需要交割条件？
- 是否需要陈述保证、赔偿、托管、回购、反稀释、重大事项保护？
- 是否需要律师、会计师、税务师、专利代理人或行业专家复核？
- 是否转成投后 100 天计划？

## 方法来源

本 Skill 综合了五本本地尽调资料的方法论：

- 《财务、法律、业务尽职调查全流程实务操作指南》：完整 DD 分类、业务/财务/法律流程、资料清单和报告模板。
- 《财务尽职调查：全流程方法与实务案例》：财务尽调、现场工作、访谈、第三方验证、订单-收入-回款交叉验证、QoE 报告逻辑。
- 《私募股权投资和尽职调查手册》：PE 投资决策、估值、谈判、交易条款和投资报告语言。
- 《投资尽职调查：投资逻辑、尽调方法、实战案例》：价值/估值/退出/风险框架，业务-财务-行业三角验证。
- 《尽职调查白皮书》：经典尽调流程、方法、公司历史、产品、资产、人力、财务、业务、法律、合同、诉讼、环保、IP 清单。

本仓库只包含对方法论的综合抽象和可执行工作流，不包含原书正文。

## 工作流

完整 DD 报告建议按以下顺序执行：

1. **Intake**
   - 确认项目名称、交易类型、决策阶段、投资角色、输出格式、资料来源。

2. **Material Inventory**
   - 盘点 BP/CIM、财务表、合同、数据室、会议纪要、访谈、公开信息、第三方报告。

3. **Basic Information Pack**
   - 抽取主体基础信息、历史沿革、股权治理、交易事实、产品、团队、财务基础和资料冲突。

4. **Investment Thesis**
   - 先写清楚“这个交易为什么可能成立”和“必须为真的关键假设”。

5. **Adapter Selection**
   - 根据交易类型选择 VC、成长股权、Pre-IPO、并购、战略投资等适配器。
   - 根据行业选择硬科技、半导体、SaaS、制造、消费、医药等适配器。

6. **Book Fusion Coverage**
   - 检查每个模块是否融合了五本书的必要视角。

7. **Hypothesis Tree**
   - 把投资逻辑拆成业务、行业、财务、法律、团队、估值、退出、投后等可验证问题。

8. **Evidence Matrix**
   - 把每个重要判断绑定到证据、来源、状态、缺口和交易影响。

9. **Triangulation**
   - 业务、行业、财务、客户、订单、回款、法律、团队相互校验。

10. **Valuation / Return / Exit / Terms**
    - 评估估值方法、回报情景、退出路径和条款保护。

11. **Red-Flag Gate**
    - 按 P0/P1/P2 标记风险，并写明交易动作。

12. **HTML Report Draft**
    - 生成结论先行、证据可追踪、表格充分的 standalone HTML。

13. **Final QA**
    - 解析 HTML、扫描敏感内容、检查桌面和移动端可读性。

## 默认输出

除非用户另有要求，完整报告应包括：

- 执行摘要和投资建议
- 交易背景和资料边界
- 基础信息与历史沿革
- 股权结构、治理、激励和交易条款
- 投资逻辑和关键假设
- 行业与市场尽调
- 产品、技术和商业模式尽调
- 客户、收入、订单、渠道和供应链尽调
- 财务尽调 / QoE
- 法律、税务、合规和交易风险
- 管理层和组织能力
- 估值、回报和退出
- 红旗登记表
- 资料缺口清单
- 交割条件和投后 100 天计划
- 最终建议和决策情景

## HTML 报告要求

完整 HTML 报告应满足：

- 单文件 standalone HTML
- inline CSS
- 有封面/hero、目录、章节 ID
- 表格充分，尤其是基础信息、股权、条款、红旗、资料缺口
- 桌面端无页面级横向溢出
- 移动端表格可在 section 内横向滚动
- 无明显文字重叠
- 不暴露原始敏感信息

推荐生成后运行：

```bash
python3 - <<'PY'
from html.parser import HTMLParser
from pathlib import Path
p = Path("REPORT.html")
class P(HTMLParser):
    pass
parser = P()
parser.feed(p.read_text(encoding="utf-8"))
print("HTML parser OK", p.stat().st_size)
PY
```

敏感内容扫描示例：

```bash
rg -n '身份证|tenant_access_token|app_ticket|token=|internal-api|user-id|银行账号' REPORT.html || true
```

## 证据与红旗规则

### 证据等级

优先级从高到低：

1. 官方原始文件：审计报告、银行流水、税务申报、合同、发票、验收单、许可证、法院/监管记录。
2. 第三方确认：客户/供应商访谈、银行确认、专家访谈、政府/工商查询、外部律师/会计师报告。
3. 内部系统导出：ERP、CRM、订单台账、仓库、工资、项目系统、生产记录。
4. 管理报表和明细表。
5. 管理层访谈、BP/CIM 口径。
6. 媒体、市场材料、传闻。

管理层口径只能形成假设，不能直接成为结论。

### 红旗等级

- **P0**：潜在 deal-stopper 或必须立即升级。
- **P1**：影响估值、条款、交割条件或专业复核。
- **P2**：投后监控或整改事项。

每个 P0/P1 必须有交易动作。

## 安装方式

### 安装到 Codex Skills

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/noahnan-max/private-equity-investment-dd-skill.git ~/.codex/skills/private-equity-investment-dd
```

如果已经 clone 到其他路径，也可以复制：

```bash
rsync -a private-equity-investment-dd-skill/ ~/.codex/skills/private-equity-investment-dd/
```

### 验证 Skill 文件

如果本地有 Codex skill-creator 校验脚本：

```bash
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py ~/.codex/skills/private-equity-investment-dd
```

## 使用示例

### 生成完整 HTML 尽调报告

```text
请使用 private-equity-investment-dd skill，基于我提供的 BP、访谈记录、会议纪要、财务表和合同，生成一份完整的 HTML 投资尽调报告。
```

### 做红旗扫描

```text
这家公司收入增长很快，但应收账款也快速增长。请基于资料做 PE 项目红旗扫描，输出风险等级、证据、交易影响和下一步查验清单。
```

### 做 Pre-IPO 项目 IC Memo

```text
这是一个半导体 Pre-IPO 项目，请基于 BP、审计报告、客户订单和管理层访谈生成 IC Memo，并重点检查收入质量、客户集中度、产能、IP 和上市退出可行性。
```

### 补充基础信息

```text
报告里的基础信息太薄了，请重新抽取主体信息、历史沿革、股权结构、治理、交易条款、产品、团队、财务基础和资料缺口。
```

## 仓库结构

```text
private-equity-investment-dd-skill/
├── README.md
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── basic-information-extraction.md
    ├── book-fusion-coverage.md
    ├── evidence-and-red-flags.md
    ├── html-report-output.md
    ├── industry-dd-adapters.md
    ├── interview-and-data-room.md
    ├── module-checklists.md
    ├── red-flag-playbook.md
    ├── report-structure.md
    ├── report-writing-examples.md
    ├── self-test.md
    ├── source-books.md
    ├── special-dd-adapters.md
    ├── valuation-and-terms.md
    └── workflow.md
```

## 安全与合规边界

不要在用户可见报告中暴露：

- 身份证号、护照号等个人敏感 ID
- 银行账号、签名、印章扫描件
- 私人地址、手机号、邮箱
- Feishu/Lark 内部文档 ID、用户 ID、内部 API URL
- token、app ticket、tenant access token、密钥
- 未脱敏合同原文和保密交易条款

建议写法：

- “源文件包含该编号，报告正文已脱敏。”
- “完整证据见底稿，本文仅保留摘要。”
- “该事项需律师/会计师/专利代理人复核。”

## 维护建议

后续可以继续扩展：

- 增加更多行业 adapter：新能源、跨境电商、AI 应用、机器人、医疗服务、消费品牌。
- 增加脚本：HTML 报告生成模板、敏感信息扫描器、证据矩阵 CSV 转 HTML。
- 增加案例测试集：早期硬件、SaaS、制造业并购、Pre-IPO、现金流异常项目。
- 增加 Word/PDF 导出流程。

---

# English Documentation

## Overview

Private Equity Investment Due Diligence Skill is a Codex skill for PE, VC/growth equity, M&A, strategic investment, Pre-IPO, and other non-public-company investment diligence workflows.

It turns messy project materials such as pitch decks, CIMs, management interviews, meeting notes, financial statements, contracts, data-room files, cloud documents, and local working papers into professional investment due diligence reports, IC memos, red-flag scans, data request lists, and interview guides.

For full reports, the default deliverable is a **standalone HTML due diligence report** with a clear evidence boundary, basic company information, investment judgment, red flags, data gaps, and transaction implications.

## When To Use

Use this skill for:

- private equity due diligence reports;
- VC/growth equity preliminary diligence;
- Pre-IPO investment review;
- buyout, M&A, minority investment, and strategic investment;
- IC memos and investment committee materials;
- red-flag scans;
- data-room request lists;
- management/customer/supplier/employee/expert interview guides;
- financial due diligence and QoE-style drafts;
- valuation, return, exit, and term-sheet analysis;
- post-investment 100-day plans.

## When Not To Use

This skill is not the primary tool for:

- public-company annual-report red-flag scoring;
- secondary-market stock recommendations;
- final legal opinions, audit reports, tax opinions, or patent opinions;
- professional sign-off on legal, tax, IP, labor, environmental, safety, litigation, or regulatory matters.

For specialist areas, the skill identifies risks and required follow-up. It does not replace lawyers, accountants, tax advisors, patent agents, or other regulated professionals.

## What Makes It Different

### 1. Mandatory Basic Information Extraction

A full report must preserve factual diligence material, including:

- material boundary and evidence status;
- legal entity basics;
- history and milestones;
- pre- and post-transaction cap tables;
- governance, ESOP, shareholder platforms, and investor rights;
- investment amount, valuation, ownership, instrument, closing conditions, and use of proceeds;
- product lines and stage;
- team and organization;
- finance basics such as revenue status, cash, burn rate, debt, and financing runway;
- source conflicts and missing materials.

### 2. Five-Book Method Fusion

The skill fuses five diligence lenses:

| Lens | Role |
| --- | --- |
| PE decision and deal terms | Whether to invest, how to price, how to protect downside |
| Investment logic triangulation | Business, finance, and industry cross-checks |
| Financial diligence / QoE | Orders, revenue, collections, cash flow, working capital, forecasts |
| Comprehensive business/legal/financial DD | Entity, equity, contracts, assets, IP, labor, tax, compliance |
| Classic checklist and workpaper discipline | Material scope, interviews, bottom papers, review, archive |

### 3. HTML-First Full Reports

Full reports default to standalone HTML so they can be opened locally, circulated internally, converted to PDF, or archived.

The HTML report emphasizes:

- conclusion-first writing;
- table-based factual organization;
- evidence status labels;
- red flags and deal actions;
- desktop and mobile readability;
- no exposure of raw sensitive identifiers.

### 4. Transaction Implication Discipline

Every serious issue must translate into one or more actions:

- stop;
- pause pending evidence;
- reprice;
- condition precedent;
- representation and warranty;
- indemnity;
- escrow or holdback;
- governance right;
- specialist review;
- post-investment action.

## Workflow

1. **Intake**
   - Identify project name, deal type, decision stage, investor role, output format, and material sources.

2. **Material Inventory**
   - Classify pitch decks, financials, contracts, data-room files, interviews, public information, and third-party reports.

3. **Basic Information Pack**
   - Extract legal entity facts, milestones, ownership, governance, transaction facts, products, team, finance basics, and source conflicts.

4. **Investment Thesis**
   - Write what must be true for the deal to work.

5. **Adapter Selection**
   - Select transaction/stage and industry adapters.

6. **Book Fusion Coverage**
   - Check whether each module uses the relevant diligence lens.

7. **Hypothesis Tree**
   - Break the deal thesis into testable business, financial, legal, team, valuation, exit, and post-investment questions.

8. **Evidence Matrix**
   - Map every important claim to evidence, source, status, gap, and deal implication.

9. **Triangulation**
   - Cross-check business claims, financial data, industry evidence, customers, orders, collections, legal documents, and team interviews.

10. **Valuation / Return / Exit / Terms**
    - Review valuation method fit, downside/upside cases, exit feasibility, and terms needed to protect against unresolved risks.

11. **Red-Flag Gate**
    - Classify P0/P1/P2 issues and define required deal actions.

12. **HTML Report Draft**
    - Produce a standalone HTML report.

13. **Final QA**
    - Validate HTML parsing, scan sensitive content, and check desktop/mobile readability.

## Default Report Structure

A full report should include:

- executive judgment;
- deal context and material boundary;
- basic company information and milestones;
- equity, governance, incentives, and transaction facts;
- investment thesis and assumptions;
- market and industry diligence;
- product, technology, and business model diligence;
- customer, revenue, order, channel, and supply-chain diligence;
- financial diligence / QoE;
- legal, tax, compliance, and transaction risk;
- management and organization;
- valuation, return, and exit;
- red-flag register;
- data request list;
- closing conditions and post-investment 100-day plan;
- final recommendation and decision scenarios.

## HTML Report Requirements

A full HTML report should be:

- a single standalone HTML file;
- styled with inline CSS;
- structured with a cover/hero, table of contents, and section IDs;
- table-heavy for facts, cap tables, terms, red flags, and data gaps;
- readable on desktop and mobile;
- safe from raw sensitive identifiers.

Validation example:

```bash
python3 - <<'PY'
from html.parser import HTMLParser
from pathlib import Path
p = Path("REPORT.html")
class P(HTMLParser):
    pass
parser = P()
parser.feed(p.read_text(encoding="utf-8"))
print("HTML parser OK", p.stat().st_size)
PY
```

Sensitive-content scan example:

```bash
rg -n 'ID card|passport|tenant_access_token|app_ticket|token=|internal-api|user-id|bank account' REPORT.html || true
```

## Evidence And Red-Flag Rules

### Evidence Hierarchy

Prefer higher-quality evidence:

1. official original documents;
2. third-party confirmations;
3. internal system exports;
4. management accounts and schedules;
5. management interviews or pitch-deck claims;
6. media, marketing materials, or hearsay.

Management claims should create hypotheses, not conclusions.

### Red-Flag Severity

- **P0**: potential deal-stopper or must-escalate issue.
- **P1**: price, term, condition precedent, or specialist-review issue.
- **P2**: monitoring or post-investment action.

Every P0/P1 issue must have a deal implication.

## Installation

Clone into the Codex skills directory:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/noahnan-max/private-equity-investment-dd-skill.git ~/.codex/skills/private-equity-investment-dd
```

Or copy the repository:

```bash
rsync -a private-equity-investment-dd-skill/ ~/.codex/skills/private-equity-investment-dd/
```

Validate if the local skill validator is available:

```bash
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py ~/.codex/skills/private-equity-investment-dd
```

## Example Prompts

### Full HTML DD Report

```text
Use the private-equity-investment-dd skill to generate a full HTML investment due diligence report based on the pitch deck, interviews, meeting notes, financials, and contracts I provided.
```

### Red-Flag Scan

```text
The company has fast revenue growth, but receivables are also rising quickly. Please run a PE red-flag scan and output severity, evidence, deal implication, and next verification steps.
```

### Pre-IPO IC Memo

```text
This is a semiconductor Pre-IPO deal. Based on the deck, audit report, customer orders, and management interviews, generate an IC memo focused on revenue quality, customer concentration, capacity, IP, and exit feasibility.
```

## Repository Structure

```text
private-equity-investment-dd-skill/
├── README.md
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── basic-information-extraction.md
    ├── book-fusion-coverage.md
    ├── evidence-and-red-flags.md
    ├── html-report-output.md
    ├── industry-dd-adapters.md
    ├── interview-and-data-room.md
    ├── module-checklists.md
    ├── red-flag-playbook.md
    ├── report-structure.md
    ├── report-writing-examples.md
    ├── self-test.md
    ├── source-books.md
    ├── special-dd-adapters.md
    ├── valuation-and-terms.md
    └── workflow.md
```

## Safety Boundary

Do not expose in user-facing reports:

- personal IDs;
- bank accounts, signatures, or stamp scans;
- private addresses, phone numbers, or emails;
- Feishu/Lark internal document IDs or user IDs;
- internal API URLs, tokens, app tickets, tenant access tokens, or secrets;
- unredacted contracts or confidential transaction clauses.

Use summaries or redaction notes instead.

## Maintenance Ideas

Potential future extensions:

- more industry adapters such as robotics, AI applications, renewable energy, cross-border ecommerce, and healthcare services;
- scripts for HTML report generation, sensitive-content scanning, and evidence-matrix conversion;
- case test sets for early-stage hardware, SaaS, manufacturing M&A, Pre-IPO, and cash-flow-stress deals;
- Word/PDF export workflows.
