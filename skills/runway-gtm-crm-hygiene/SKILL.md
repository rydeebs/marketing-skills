---
name: runway-gtm-crm-hygiene
description: "Audit and clean GTM CRM records, including self-serve signups, product-qualified leads, and enterprise accounts, while preserving attribution, consent, and relationship history."
---

# CRM hygiene

## Purpose and inputs

Audit and clean GTM CRM records, including self-serve signups, product-qualified leads, and enterprise accounts, while preserving attribution, consent, and relationship history.

Runway (runwayml.com) builds generative video and media models and tools, sold through a self-serve web app, team and enterprise plans, and a developer API. Buyers range from individual creators and creative professionals to agencies, brand marketing teams, media and entertainment studios, gaming companies, and developers building on the API. Check current model names, features, plan tiers, pricing, usage terms, and content policy against runwayml.com, the Help Center, or internal docs before stating them. Do not rely on memory, because the lineup changes often.

Start with: CRM schema (Salesforce, HubSpot, or other), a read-only export or access, lead-source and lifecycle definitions, product-usage fields, account-matching rules, merge policy, and consent and suppression fields. Use supplied context first. Ask only for missing facts that block a correct result; mark other gaps and continue.

## Workflow

1. Inspect the schema and take a scoped pre-change export when allowed. Profile missing sources, duplicate leads and accounts, unmatched self-serve users, inconsistent stages, and unstructured lost reasons.

2. Propose matching rules using strong identifiers such as email domain, workspace ID, and billing account. Do not merge on name alone, and handle personal-email signups and agency users who work across client accounts carefully.

3. Map canonical sources and stages, and draft field-level changes with record IDs, old values, proposed values, rationale, and confidence. Keep original attribution next to corrected fields.

4. Apply only authorized, reversible changes in bounded batches. Verify changed counts and sample records against the plan, keep a rollback map, and stop on unexpected conflicts.

## Deliverable

Deliver an audit summary, duplicate-review queue, field mapping, proposed or verified change log, and segment definitions for eligible lifecycle and sales-assist audiences.

## Quality checks

Never erase consent, suppression, activity history, or first-touch attribution to make a record look clean. Leave ambiguous merges for human review, and never infer marketing permission from a product signup. Never overstate model capabilities or show cherry-picked generations as typical output without saying so. Respect likeness, voice, and IP rights in any generated or customer media, follow Runway’s content policy and AI-disclosure norms, and keep NDA’d customer, studio, and partner names out of public material without written approval.

## Execution boundary

Use the tools available in the working environment; if access is missing, deliver a usable draft or handoff and state the limitation. Follow the user’s existing authorization and tool policies. Before any external change or communication, confirm the account, destination, and scope; this skill itself grants no authority to publish, send, purchase, or delete. Record confirmed results and stop after at most two retries of a failed write unless the service proves it did not land.

## Source

Adapted for a Runway go-to-market role from the “CRM hygiene” workstream in [Jameson Haslam’s remote marketing playbook](https://x.com/jamesonhaslam/status/2098453252618731882). The original post supplies the topic; the workflow, checks, and deliverable specification here are an adaptation, not an endorsement or a revenue guarantee.
