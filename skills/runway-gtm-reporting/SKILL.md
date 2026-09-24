---
name: runway-gtm-reporting
description: "Build a weekly GTM scorecard for Runway that reconciles signups, activation, paid conversion, pipeline, and revenue by source, with explicit attribution limits."
---

# GTM reporting

## Purpose and inputs

Build a weekly GTM scorecard for Runway that reconciles signups, activation, paid conversion, pipeline, and revenue by source, with explicit attribution limits.

Runway (runwayml.com) builds generative video and media models and tools, sold through a self-serve web app, team and enterprise plans, and a developer API. Buyers range from individual creators and creative professionals to agencies, brand marketing teams, media and entertainment studios, gaming companies, and developers building on the API. Check current model names, features, plan tiers, pricing, usage terms, and content policy against runwayml.com, the Help Center, or internal docs before stating them. Do not rely on memory, because the lineup changes often.

Start with: Reporting window and timezone, product analytics, billing data, CRM pipeline, marketing-automation and ad data, web analytics, content and event logs, and a prior-period baseline. Use supplied context first. Ask only for missing facts that block a correct result; mark other gaps and continue.

## Workflow

1. Define each metric: signup, activated user, paid conversion, MQL/PQL, SQL, opportunity, pipeline, bookings, and ARR. Align date fields, timezone, and whether the report uses event dates or signup cohorts.

2. Reconcile unique users and accounts across product, billing, and CRM with stable IDs. Keep an unknown-source bucket, and do not credit one conversion to several channels in a single-source total.

3. Report self-serve funnel, sales-assist and enterprise pipeline, API usage, channel performance, launches, and events. Separate activity inputs from business outcomes.

4. Compare with a consistent prior period. Explain material changes with evidence or label them as hypotheses, and call out missing data, small samples, seasonality, launch spikes, and conversion lag before recommending action.

## Deliverable

Deliver a compact weekly scorecard with metric, definition, current, prior, change, source, and caveat, plus the most important findings and next actions with owners.

## Quality checks

Show unavailable values as unknown, not zero. Show percentages with denominators, weight averaged conversion rates, and keep bookings, billed revenue, and collected revenue distinct. Never overstate model capabilities or show cherry-picked generations as typical output without saying so. Respect likeness, voice, and IP rights in any generated or customer media, follow Runway’s content policy and AI-disclosure norms, and keep NDA’d customer, studio, and partner names out of public material without written approval.

## Execution boundary

Use the tools available in the working environment; if access is missing, deliver a usable draft or handoff and state the limitation. Follow the user’s existing authorization and tool policies. Before any external change or communication, confirm the account, destination, and scope; this skill itself grants no authority to publish, send, purchase, or delete. Record confirmed results and stop after at most two retries of a failed write unless the service proves it did not land.

## Source

Adapted for a Runway go-to-market role from the “Marketing reporting” workstream in [Jameson Haslam’s remote marketing playbook](https://x.com/jamesonhaslam/status/2098453252618731882). The original post supplies the topic; the workflow, checks, and deliverable specification here are an adaptation, not an endorsement or a revenue guarantee.
