# TacoLang Context Library — Deferred Feature

## Concept

Expand `emtinker.com/tacolang` from a single redirect into a path-based contextual library.
Agents load the spec AND domain-specific briefs before starting a research thread.

## Proposed URL Structure

```
emtinker.com/tacolang                        → SPEC.md (language spec)
emtinker.com/tacolang/context/security       → security research brief
emtinker.com/tacolang/context/forensics      → forensics methodology + tool list
emtinker.com/tacolang/context/legal          → legal research framing doc
emtinker.com/tacolang/context/<topic>        → any domain brief
```

## Agent Thread Header (future)

```
AGENT::CONTEXT::tacolang → LOADED
AGENT::CONTEXT::forensics → LOADED
ref: https://emtinker.com/tacolang/context/forensics
```

## Implementation

- Replace Cloudflare 301 redirect with a static site (Cloudflare Pages or GitHub Pages)
- Each path serves a markdown document
- No backend required — purely static
- Cloudflare Pages deploys directly from the emtinker/tacolang repo

## Status

DEFERRED — current 301 redirect is sufficient for now.
Revisit when credits are plentiful.
