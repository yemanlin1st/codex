# Secure MCP Tool Use Workflow

## Purpose

Use MCP-inspired interoperability without creating uncontrolled tool risk.

## Rule

Deny by default. Allow only reviewed tools, reviewed resources and reviewed actions.

## Workflow

1. Understand the user request.
2. Confirm whether a tool is truly needed.
3. Select an approved tool/server from the registry.
4. Check permission scope.
5. Check data sensitivity.
6. Use read-only access first when possible.
7. Require explicit human approval for write, send, delete, deploy, publish, payment or sensitive actions.
8. Record the action in an audit log when operationalized.
9. Return a clear, zero-noise result.

## Block conditions

Block or escalate when:

- the server is unknown;
- the action is not allowlisted;
- the request includes secrets or sensitive client data;
- the action is irreversible;
- the tool could exfiltrate data;
- the result depends on unverified external claims;
- the user intent is ambiguous and the action is sensitive.

## Safe defaults

- read before write;
- least privilege;
- scoped access;
- public-safe commits only;
- no secrets in repositories;
- no silent automation;
- no broad connector access without clear need.
