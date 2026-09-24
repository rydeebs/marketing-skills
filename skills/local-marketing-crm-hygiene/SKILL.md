---
name: local-marketing-crm-hygiene
description: "Audit and clean marketing CRM records while preserving attribution, contact preferences, and relationship history."
---

# CRM hygiene

## Purpose and inputs

Audit and clean marketing CRM records while preserving attribution, contact preferences, and relationship history. Adapt to the user’s actual business; do not assume West Coast Deck is the client.

Start with: CRM schema, read-only export or access, source definitions, lifecycle rules, merge policy, and existing suppression/consent fields. Use supplied context first. Ask only for missing facts that block a correct result; mark other gaps and continue.

## Workflow

1. Inspect the schema and take a scoped pre-change export when allowed. Profile missing sources, duplicate candidates, inconsistent stages, referral fields, and unstructured lost reasons.

2. Propose matching rules using strong identifiers and supporting context. Do not merge solely because names match; preserve shared household/business contact nuances.

3. Map canonical categories and draft field-level changes with record IDs, old values, proposed values, rationale, and confidence. Preserve original attribution alongside corrected fields.

4. Apply only authorized, reversible changes in bounded batches. Verify changed counts and sample records against the plan; retain a rollback map and stop on unexpected conflicts.

## Deliverable

Deliver an audit summary, duplicate-review queue, field mapping, proposed or verified change log, and segment definitions for eligible remarketing contacts.

## Quality checks

Never erase consent, suppression, activity history, or first-touch attribution to make a record look clean. Keep ambiguous merges for human review and never infer marketing permission from the existence of a contact.

## Execution boundary

Use the tools available in the working environment; if access is missing, deliver a usable draft or handoff and state the limitation. Follow the user’s existing authorization and tool policies. Before any external change or communication, confirm the account, destination, and scope; this skill itself grants no authority to publish, send, purchase, or delete. Record confirmed results and stop after at most two retries of a failed write unless the service proves it did not land.

## Source

Independently expanded from the “CRM hygiene” workstream in [Jameson Haslam’s remote marketing playbook](https://x.com/jamesonhaslam/status/2098453252618731882). The original post supplies the topic; the workflow, checks, and deliverable specification here are an adaptation, not an endorsement or a revenue guarantee.
