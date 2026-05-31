# TacoLang v0.1

A structured communication protocol for agent-to-agent and human-to-agent interactions.

---

## Syntax

```
AGENT::ACTION::TARGET → RESULT
```

## Fields

| Field | Description | Format |
|-------|-------------|--------|
| AGENT | Who is acting | Uppercase identifier (e.g. USER, AGENT-A, AGENT-B) |
| ACTION | What they are doing | SCREAMING_SNAKE_CASE verb |
| TARGET | What is being acted on | file, dir, system, concept, or endpoint |
| RESULT | Outcome or state after the action | optional but preferred |

## Common Actions

| Action | Meaning |
|--------|---------|
| ADD | Create or introduce something new |
| REMOVE | Delete or purge something |
| FIX | Repair a broken thing |
| REFACTOR | Restructure without changing behavior |
| AUDIT | Security or quality review |
| DEPLOY | Push to production or a live environment |
| WIRE | Connect two systems or agents |
| UPDATE | Modify an existing thing |
| RESEARCH | Investigate a topic |
| FILE | Archive a finding or record |
| BRIEF | Deliver a summary or context packet |
| FLAG | Surface a concern or anomaly |

## Examples

```
USER::REFACTOR::repository → NAMESPACE_STRUCTURED
AGENT::AUDIT::functions/webhook → SECRETS_CLEAN
AGENT::DEPLOY::narrate_endpoint → SERVICE_LIVE
AGENT::RESEARCH::topic → FINDINGS_READY
AGENT::FILE::record_summary → ARCHIVED
```

## Multi-line Format

Use a primary TacoLang line as the subject, then bullet details in the body:

```
AGENT::WIRE::service_tunnel → CONNECTED

- Access policy enforced
- Endpoint verified: returning 200 with auth headers
- Token stored in service daemon
```

## Record Summaries

When an agent concludes a research thread, output a Record Summary:

```
AGENT::RESEARCH::topic → FINDING_DISTILLED

[2-3 sentence distilled finding, ready for archiving.]
```

## Thread Header

Begin new agent threads with:

```
AGENT::CONTEXT::tacolang → LOADED
ref: https://emtinker.com/tacolang
```

---

Human contributions use the same syntax. Humans are agents too.
