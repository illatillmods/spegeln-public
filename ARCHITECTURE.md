# Public Architecture Overview

This overview explains the product shape while keeping source code, prompts,
data schemas, deployment configuration and implementation algorithms private.

## Product Layers

- Web product: accounts, privacy, authority intelligence, reports, civic action,
  pricing and operational status.
- API service: authentication, API keys, payments, evidence metadata, report
  intake and civic workflows.
- Analysis worker: AI classification, extraction, summaries, triage and drafting.
- Data layer: source-linked records, users, reports, authorities, payments,
  API consumers and public correction history.
- Evidence storage: private originals, public derivatives and source archives
  with their respective access controls.

## Product Rules

- Verified public records publish automatically with source attribution.
  Uploaded evidence receives AI labels and specified exception handling before
  publication. Suspected manipulated media has a separate authenticity check.
  (FD-008, FD-010, FD-011)
- Unsubstantiated claims and AI-derived relationships stay distinct from
  evidence. Legal review advises without a publication veto. (FD-008, FD-012,
  FD-045)
- The app stores no IP addresses or raw device data about anonymous tipsters;
  case tokens and normal operational minimum remain. Providers' short security
  logs are minimized. (FD-120, FD-199)
- Civic actions use the user's chosen scope without fixed recipient or volume
  caps. Delivery failures and retries remain visible. (FD-017, FD-068)
- Free API registration is direct; premium access activates after payment.
  (FD-098, FD-172)
- Failed AI work is queued with visible status. (FD-174, FD-196)
- Built, partly built and planned functions are labelled separately. (FD-109)

## Not Published Here

This mirror excludes endpoint implementations, prompt text, connector code,
database schemas, deployment topology, infrastructure names and operational
runbooks. It remains a separate documentation repository.
