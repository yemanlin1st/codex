# Top 5 MCP Benchmark for PEA Account V9.2

Date: 2026-06-16
Repository: yemanlin1st/codex
Reference: PEA Account Kernel V9.2

## Purpose

Select the 5 MCP capability classes that are truly useful for this account. The objective is not to install many tools. The objective is to improve continuity, memory, GitHub operations, research, documentation, productivity and controlled execution.

## Selection criteria

Each MCP capability was assessed against:

- usefulness for PEA/V9 account operations;
- contribution to memory continuity;
- contribution to GitHub/source-of-truth workflows;
- risk level;
- security controllability;
- low-cost potential;
- portability;
- productivity gain;
- relevance for revenue, consulting, documents, code and dashboards.

## Recommended top 5

### 1. GitHub MCP

Use for repository management, file operations, pull requests, code/document review, AGENTS/SKILL/workflow management and source-of-truth governance.

Value for this account: very high.

Controls:
- read first;
- write only with explicit approval;
- no secrets;
- public-safe commits only;
- prefer branches/PRs for large changes.

### 2. Filesystem and Git MCP

Use for local workspace navigation, file editing, pack generation, local repo maintenance and offline-first work.

Value for this account: very high.

Controls:
- restrict root directory;
- no access to home-wide filesystem by default;
- no shell execution unless specifically approved;
- maintain backups before bulk changes.

### 3. PostgreSQL / MemCash MCP

Use for structured memory, project nodes, archive retrieval, CRM data, KPIs, dashboards, audit logs and future PEA/SCPro/EULYONIS data models.

Value for this account: very high.

Controls:
- read-only default;
- separate public/private/confidential schemas;
- use RLS where applicable;
- no sensitive personal data in public memory;
- backups and audit logs required.

### 4. Google Drive / Docs MCP

Use for documents, reports, proposals, decks, client files, knowledge retrieval and continuity across document-heavy workflows.

Value for this account: high.

Controls:
- least privilege;
- read-only by default;
- explicit approval before editing, sharing or deleting;
- classify files before processing;
- avoid mixing confidential client material into public repos.

### 5. Web Search / Browser / Fetch MCP

Use for benchmark, current information, standards, market research, competitive intelligence, product research and evidence checks.

Value for this account: high.

Controls:
- cite sources;
- cross-check important claims;
- no blind scraping;
- no paywall bypass;
- no unsafe browsing automation;
- separate facts from assumptions.

## Not top 5 for now

### Stripe / Payment MCP

Useful later for revenue, invoicing and subscription workflows, but too sensitive for early activation. Keep blocked until financial governance and approval controls are ready.

### Slack / Messaging MCP

Useful for team operations, but risk of private data exposure and message mistakes is high. Use only after workspace classification and approval rules.

### Browser automation / Puppeteer MCP

Useful for QA and visual testing, but risky if used broadly. Keep sandboxed and task-specific.

## Final ranking

| Rank | MCP capability | Usefulness | Risk | Decision |
|---|---|---|---|---|
| 1 | GitHub | Very high | Medium | Approve with controls |
| 2 | Filesystem/Git | Very high | Medium/High | Approve in sandbox |
| 3 | PostgreSQL/MemCash | Very high | Medium/High | Approve with schema/RLS |
| 4 | Google Drive/Docs | High | High | Approve read-first |
| 5 | Web Search/Fetch | High | Medium | Approve with citations |

## Integration rule

PEA V9.2 must use MCP as a secure interoperability layer, not as uncontrolled autonomy.

Operating formula:

```text
Need-based request
+ approved MCP capability
+ least privilege
+ human approval for sensitive actions
+ audit log
+ zero-noise output
= useful and safe account improvement
```

## Next implementation tasks

- [ ] Add GitHub MCP to approved registry.
- [ ] Add Filesystem/Git MCP sandbox policy.
- [ ] Add PostgreSQL/MemCash schema policy.
- [ ] Add Google Drive/Docs access policy.
- [ ] Add Web Search/Fetch evidence policy.
- [ ] Keep Stripe, Slack and broad browser automation blocked until governance is ready.
