# Public Architecture Overview

This overview is intentionally high-level. It explains the product shape without
publishing source code, prompts, data schemas, deployment configuration or
algorithms that would make the product cloneable.

## Product Layers

- Web product: account, privacy, authority intelligence, reports, civic action,
  pricing and admin-facing operational views.
- API service: authentication, public API keys, review queues, payments,
  evidence metadata, report intake and civic workflow endpoints.
- Analysis worker: private AI-assisted classification, extraction, summaries,
  triage and drafting support.
- Data layer: relational records for users, reports, authorities, review state,
  payment state, API consumers and audit-oriented events.
- Evidence storage: private object/file storage for uploaded evidence and media
  references, with review and access controls handled outside this mirror.

## Trust Controls

The private implementation is organized around:

- review state before public claims
- pseudonymous submission rather than unsupported anonymity claims
- bounded batch actions with rate limits and recipient caps
- scoped API keys instead of open bulk access
- separation between private evidence, operational review and public summaries
- environment-controlled publication posture for sensitive report flows

## Not Published Here

This mirror deliberately excludes endpoint implementations, prompt text,
connector code, scoring formulas beyond public-safe summaries, database schema
details, deployment topology, infrastructure names and operational runbooks.
