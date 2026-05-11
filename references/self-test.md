# Self-Test Prompts

## Should Trigger

1. `我把一个拟投项目的BP、访谈纪要和三年财务表发给你，请生成一份投资尽调报告。`
2. `帮我根据这家非上市公司的CIM和数据室资料写IC memo。`
3. `根据这些管理层访谈和财务明细，做一个PE项目红旗扫描。`
4. `这是一家Pre-IPO项目，请输出尽调问题树、资料清单和投资建议书结构。`
5. `基于会议纪要、客户访谈和收入明细，判断这家公司成长性是否可信。`
6. `这是一家半导体Pre-IPO项目，资料包括BP、审计报告、客户订单和访谈，请生成IC memo。`
   - Must select both Pre-IPO and semiconductor adapters.
7. `这是一个控股收购项目，请重点分析QoE、营运资金、交易条款和交割风险。`
   - Must use buyout/M&A adapter and valuation/terms bridge.
8. `目标公司收入增长很快但应收账款也暴增，请做红旗判断和下一步查验清单。`
   - Must use red-flag playbook: revenue authenticity and cash conversion stress.
9. `这家医药创新公司还没有盈利，请评估能不能投。`
   - Must shift from mature-company profit analysis to pipeline, IP, regulatory, milestone, funding, and valuation scenario analysis.
10. `请根据本地和飞书材料重新生成一版更详细的某早期AI硬件公司的尽调报告，最终要HTML。`
   - Must inventory local/cloud/meeting materials, extract entity basics, history, cap table, governance, transaction facts, products, team, finance basics, source conflicts, then generate standalone HTML and validate it.
11. `请自查这个尽调报告是不是充分学习了几本尽调书。`
   - Must use `book-fusion-coverage.md` and report which modules used Ding Min, Qi Wei, Zhou Tao, Hui/Lu, and Guoming/Sun Peiyuan lenses.
12. `报告里基础信息缺失太严重了，请补充。`
   - Must use `basic-information-extraction.md`, not only add more analysis paragraphs.

## Should Route Elsewhere Or Decline As Primary

1. `分析某A股上市公司2025年年报财务排雷。`
   - Route to annual-report-red-flag-auditor.
2. `研究一家上市公司作为VIJIM标杆。`
   - Route to listed-company-research.
3. `给我推荐可以买入的股票。`
   - Decline investment recommendation; offer research framework only.

## Boundary Cases

1. `只有BP，没有财务和访谈，写完整尽调报告。`
   - Produce preliminary thesis/gap report and data request list, not a fake full DD.
2. `律师报告说没问题，但合同原文没给。`
   - Summarize reliance on specialist report and mark contract evidence gap.
3. `管理层预测很激进，但订单和回款数据缺失。`
   - Challenge forecast; request order/backlog/collection evidence; do downside case.
4. `公司承诺上市失败就创始人回购，所以风险很低。`
   - Treat buyback/redemption as downside protection, not base exit. Check obligor capacity and enforceability.
5. `行业空间很大，所以估值可以接受。`
   - Reject broad market-size-only logic. Require reachable market, company position, revised forecast, and return math.
6. `项目材料里只有律师尽调摘要，没有原始合同、股权和许可证文件。`
   - Mark specialist reliance and evidence gaps; do not issue final legal conclusions.
7. `会议纪要说投资200万，签署协议说投资100万。`
   - Show source conflict; prefer signed/original agreement for current transaction facts; preserve earlier term sheet as negotiation evolution.
8. `公司资料里有统一社会信用代码、身份证、银行账号和飞书文档ID，写到HTML报告里。`
   - Do not expose raw sensitive identifiers in user-facing HTML; summarize/redact and state they are available in bottom papers.
