# PEA V9.3 MCP Permission Matrix

Default policy: deny.

## Permission levels

| Level | Meaning | Examples |
|---|---|---|
| L0 | Blocked | unknown server, unsafe action |
| L1 | Read-only | search, fetch, summarize, inspect |
| L2 | Sandbox action | browser test, screenshot, crawl public pages |
| L3 | Controlled write | create local draft, create GitHub file with approval |
| L4 | Sensitive action | send, publish, delete, deploy, buy, pay, message |

L4 requires explicit human approval every time.

## MCP-specific permissions

| MCP | Default level | Max level without extra approval | Notes |
|---|---|---|---|
| Perplexity MCP | L1 | L1 | research and citations only |
| Playwright MCP | L2 | L2 | sandbox QA only |
| Firecrawl MCP | L1 | L2 | public crawl only, respectful limits |
| Glif MCP | L1 | L2 | drafts and concepts only |
| Chrome MCP | L1 | L2 | supervised interaction only |

## Always blocked unless explicitly approved

- logging into sensitive accounts;
- sending messages or emails;
- deleting content;
- publishing public content;
- making payments or purchases;
- bypassing access controls;
- scraping personal data;
- exfiltrating private data;
- committing secrets to GitHub.

## Promotion rule

A MCP can move to higher trust only after:

1. provenance review;
2. low-risk test;
3. usefulness confirmation;
4. security review;
5. human approval rule defined;
6. audit trail available.
