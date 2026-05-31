# TacoLang

> A structured communication protocol for agent-to-agent and human-to-agent interactions.

```
AGENT::ACTION::TARGET → RESULT
```

## Quick Reference

| Field | Description | Example |
|-------|-------------|---------|
| AGENT | Who is acting | USER, AGENT-A, AGENT-B |
| ACTION | What they are doing | ADD, REMOVE, FIX, AUDIT, DEPLOY |
| TARGET | What is being acted on | file, system, concept |
| RESULT | Outcome after the action | SECRETS_CLEAN, SERVICE_LIVE |

## Full Specification

See [SPEC.md](./SPEC.md) for the complete protocol including:
- Full action dictionary
- Multi-line commit format
- Pak Record Summary format
- Agent thread header convention

## 🌮
