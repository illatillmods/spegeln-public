# Spegeln

Spegeln is a Swedish civic accountability product for following authority signals,
organizing evidence, preparing administrative actions and keeping public claims
reviewable before they are published.

This repository is a public mirror surface. It is provided for product
transparency and updates only. It does not contain source code, prompts,
datasets, ranking logic, deployment configuration or private planning material.

## Status

Spegeln is not represented here as a public open-source project. The private
codebase currently supports a beta/release-prep product surface with:

- authority and official profile views backed by open-record connectors and
  stored review data
- watchdog ingestion, review queues and cached insight dashboards
- pseudonymous report intake with moderation/review status
- evidence metadata and upload plumbing for review workflows
- constrained batch workflows for JO, GDPR, information requests and complaints
- AI-assisted triage, drafting and summarization behind private worker services
- scoped public API registration with key, scope and rate-limit controls
- account, privacy, consent, payment and admin-operational surfaces

The product should not be described as fully launched, fully anonymous,
externally certified, benchmarked, universally manually reviewed or open source.

## What Makes It Different

Spegeln is designed around a simple constraint: public accountability work has
to be traceable. The private implementation emphasizes source attribution,
review queues, audit-friendly storage models, bounded batch actions and clear
separation between private evidence, operational review and public-facing
claims.

The strongest public-safe product idea is not a single dataset or model. It is
the workflow layer: connect open signals, collect citizen evidence, keep review
state visible, and turn verified facts into controlled civic action without
exposing the internals that make the system reproduceable.

## Public-Safe Product Surface

### Authority Intelligence

Spegeln organizes authority and official profiles from configured open-source
connectors, internal records, reports and review events. Public dashboards are
described as cached and aggregate, not realtime raw surveillance feeds.

### Evidence And Review

Reports, testimonials, reverse-surveillance submissions and wiki-style entries
move through moderation or review-oriented states. Public copy should describe
these flows as pseudonymous or review-gated unless a signed legal policy says
otherwise.

### Bounded Administrative Action

Batch workflows are intentionally constrained. They use sender identity,
recipient limits, rate limits, tracking codes and transport status rather than
unbounded mass messaging.

### AI Assistance

AI is used to assist with triage, extraction, summaries, drafting and appeal
bundles. The public mirror intentionally does not publish prompts, provider
configuration, routing rules or private evaluation details.

### API Access

The public API surface is scoped and key-gated. Registration may create API keys,
but premium or partner access is a separate review path, not an automatic right
to bulk data.

## Non-Claims

This public mirror makes no claim that Spegeln has:

- public benchmark results
- SOC 2, ISO 27001 or equivalent external certification
- complete automated privacy export/deletion workflows
- universal manual review in every runtime configuration
- a production-ready public launch posture
- permission for third parties to copy, host, modify or commercialize the work

## Screenshots

Screenshots are intentionally omitted until each image is reviewed for private
data, sensitive operational context and cloneable implementation details.

## Contact

For access, press, security or partnership questions, use the contact channel
provided by the project owner. Do not treat this mirror as an invitation to copy
or rebuild the product.
