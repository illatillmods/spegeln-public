# Spegeln

Spegeln is a Swedish civic accountability product for public records, structured
evidence, review workflows, and bounded administrative pressure.

The product thesis is simple: accountability work needs memory, receipts, and
restraint. Public claims should be traceable, private evidence should stay
private, and powerful institutions should be easier to inspect without turning
the tool into an unreviewed rumor machine.

This repository is a public mirror surface. It is provided for product
transparency and updates only. It does not contain source code, prompts,
datasets, connector internals, ranking logic, deployment configuration, private
planning material, or anything needed to rebuild the private product.

## Snapshot

As of June 25, 2026, Spegeln is best described as a private beta / release-prep
product, not a fully launched public platform and not an open-source project.

The private codebase currently supports public-safe surfaces in these areas:

- authority and official profile views backed by open-record connectors and
  stored review data
- watchdog ingestion, review queues, and cached insight dashboards
- pseudonymous report intake with moderation/review status
- evidence metadata and upload plumbing for review workflows
- constrained workflows for JO, GDPR, information requests, complaints, and
  related administrative actions
- AI-assisted triage, drafting, extraction, summarization, and appeal-bundle
  preparation behind private worker services
- scoped public API registration with key, scope, and rate-limit controls
- account, privacy, consent, payment, and admin-operational surfaces

The product should not be described as fully launched, fully anonymous,
externally certified, benchmarked, universally manually reviewed, or open
source.

## Product Shape

Spegeln is not a single dataset. The stronger product idea is the workflow layer:

1. Connect open authority signals.
2. Store source and review context.
3. Collect citizen evidence without making it public by default.
4. Keep moderation and legal-review states visible to operators.
5. Turn verified facts into controlled civic action.
6. Publish only what can be defended.

The private implementation emphasizes source attribution, review queues,
audit-friendly storage models, bounded batch actions, and clear separation
between private evidence, operational review, and public-facing claims.

## Public-Safe Surface Areas

### Authority Intelligence

Spegeln organizes authority and official profiles from configured open-source
connectors, internal records, reports, and review events. Public dashboards are
described as cached and aggregate, not realtime raw surveillance feeds.

### Evidence And Review

Reports, testimonials, reverse-surveillance submissions, and wiki-style entries
move through moderation or review-oriented states. Public copy should describe
these flows as pseudonymous or review-gated unless signed legal policy says
otherwise.

### Bounded Administrative Action

Batch workflows are intentionally constrained. They use sender identity,
recipient limits, rate limits, tracking codes, and transport status instead of
unbounded mass messaging.

### AI Assistance

AI assists with triage, extraction, summaries, drafting, anomaly detection, and
appeal preparation. The public mirror does not publish prompts, provider
configuration, routing rules, or private evaluation details.

### API Access

The public API surface is scoped and key-gated. Registration may create API keys,
but premium or partner access is a separate review path, not an automatic right
to bulk data.

## Hard Non-Claims

This public mirror makes no claim that Spegeln has:

- public benchmark results
- SOC 2, ISO 27001, or equivalent external certification
- complete automated privacy export/deletion workflows
- universal manual review in every runtime configuration
- a production-ready public launch posture
- permission for third parties to copy, host, modify, or commercialize the work

## Mirror Contents

- [ARCHITECTURE.md](ARCHITECTURE.md) - public system overview without cloneable internals.
- [ROADMAP.md](ROADMAP.md) - public roadmap and launch boundaries.
- [SECURITY.md](SECURITY.md) - security and disclosure expectations.
- [FAQ.md](FAQ.md) - public answers.
- [CONTRIBUTING.md](CONTRIBUTING.md) - contribution posture.
- [NOTICE.md](NOTICE.md) - all-rights-reserved notice.
- [screenshots/](screenshots/) - reserved for reviewed public screenshots only.

Screenshots are intentionally omitted until each image is reviewed for private
data, sensitive operational context, and cloneable implementation details.

For access, press, security, or partnership questions, use the contact channel
provided by the project owner. Do not treat this mirror as an invitation to copy
or rebuild the product.
