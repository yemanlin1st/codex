# Approved MCP Registry V9.2 Summary

Default policy: deny.

Approved capability classes:

1. GitHub MCP: approved with controls.
2. Filesystem and Git MCP: approved only in sandbox.
3. PostgreSQL / MemCash MCP: approved with schema controls.
4. Google Drive / Docs MCP: approved read-first.
5. Web Search / Fetch MCP: approved with citation policy.

Blocked for now:

- Payment MCP until finance governance is ready.
- Messaging MCP until workspace classification is ready.
- Broad browser automation until sandbox rules are ready.

Global controls:

- least privilege;
- read before write;
- approval for sensitive actions;
- no secrets in public repositories;
- public, private and confidential data separation;
- audit important actions;
- anti-bias and zero-noise gates for important outputs.
