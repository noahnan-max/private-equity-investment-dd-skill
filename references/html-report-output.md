# HTML Report Output

Use this when generating a full DD report. Default to a single standalone `.html` file unless Noah asks for Markdown, DOCX, PDF, or a slide deck.

## Content Requirements

The HTML report must include:

1. cover/hero with project name, target, date, deal type, report nature, and confidentiality/internal-use note;
2. executive judgment with recommendation, thesis, upside, risk, and required actions;
3. material boundary and evidence limitation;
4. basic-information section with entity facts, history, cap table/governance, transaction facts, product/team/finance basics;
5. analytical sections from `report-structure.md`;
6. evidence-aware tables: status, source, gap, deal implication;
7. red-flag register with P0/P1/P2 severity and required action;
8. prioritized data request list;
9. post-investment or closing action plan;
10. footer stating date cutoff, scope, limitations, and specialist-verification boundary.

## Layout Rules

- Use valid standalone HTML with inline CSS.
- Prefer sober internal-report styling over marketing visuals.
- Use clear section IDs and a clickable table of contents.
- Use tables for factual material, cap tables, transaction terms, red flags, and data requests.
- For mobile, allow wide diligence tables to scroll horizontally within sections instead of compressing columns into unreadability.
- Avoid decorative clutter. The report should feel like an investment committee document, not a landing page.

## Sensitive Content Rules

Do not expose in user-facing HTML:

- raw personal IDs;
- full unified social credit codes or equivalent private identifiers unless Noah explicitly asks and it is necessary;
- bank accounts, signatures, stamps, private addresses, phone numbers, emails;
- Feishu/Lark internal document IDs, user IDs, internal API URLs, tokens, app tickets, tenant access tokens;
- raw contract pages or confidential clauses beyond necessary summary.

Use phrases such as "source material contains the identifier; redacted in report" or "available in bottom paper".

## Local Validation Checklist

After writing HTML, run at minimum:

```bash
python3 - <<'PY'
from html.parser import HTMLParser
from pathlib import Path
p = Path('REPORT.html')
class P(HTMLParser): pass
parser = P()
parser.feed(p.read_text(encoding='utf-8'))
print('HTML parser OK', p.stat().st_size)
PY
```

Then scan for sensitive content patterns relevant to the case, for example:

```bash
rg -n '身份证|tenant_access_token|app_ticket|token=|internal-api|user-id|银行账号' REPORT.html || true
```

For substantial reports, open the file in a browser and check:

- title is correct;
- sections and table of contents are present;
- desktop viewport has no page-level horizontal overflow;
- mobile viewport is readable and tables scroll inside sections;
- no obvious text overlap;
- screenshots are saved if visual QA is important.

## File Naming

Prefer:

`outputs/<project-slug>/<project-slug>-investment-dd-detailed-report.html`

For revisions:

`<project-slug>-investment-dd-detailed-report-v2.html`
