# Claustra

Private AI infrastructure for the corporate network.

Claustra runs autonomous LLM agents entirely inside your perimeter: local
inference on vLLM, per-session sandboxes, retrieval over internal documents,
and tool access through an audited MCP broker. No cloud dependency, no data
egress, and explicit trust boundaries between the control, data and
execution planes.

## Principles

- **Local by default** — models, documents and caches stay on our hardware.
- **Deny by default** — no egress, no host mounts, no Docker socket in sandboxes.
- **The model never holds credentials** — the broker injects secrets upstream.
- **Every tool call is auditable** — who, when, which session, what result.
