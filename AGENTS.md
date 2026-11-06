# Trade Skills — Agent Operating Instructions

## Purpose

This repository is a reusable operating system for apparel export sales. It is designed for AI agents and human sales operators working on prospecting, research, outreach, customer communication, quotation, sampling, negotiation, order execution, pipeline management, and sales analysis.

## Source of Truth

Read these files before using company-specific information:

1. `config/company-profile.md` — current employer / represented supplier.
2. `config/sales-context.md` — stable sales context, ICP, markets, channels, personalization rules, and evidence standards.

Company identity is intentionally separated from the Skills. If the employer changes, update the company profile only unless the workflow itself has changed.

## Skill Selection

Use the smallest useful set of Skills.

### New Prospect
`01 → 02 → 16 → 04/17 → 09`

### Targeted Brand
`02 → 16 → 17`

### Existing Buyer / Active Conversation
`07 → 18 → 09`

### Price Request
`08 → 11 → 13 (if needed) → 09`

### Sample Request
`08 → 12 → 07`

### Active Deal
`18 → 13 (if needed) → 12 → 09`

### Alibaba Problem
`06 → 14`

### Sales Review
`09 → 14 → 20 → 19`

### Company Change
Update `config/company-profile.md` first, then re-check any company-specific claims.

## Handoff Rules

Every Skill should pass forward:

- confirmed facts
- buyer/company context
- unknowns
- assumptions or hypotheses
- buyer intent / buying signals
- commercial constraints
- next recommended action
- evidence or source when external research was used

Do not silently convert a hypothesis into a fact.

## Evidence Labels

Use:

- **Verified** — directly confirmed by a reliable source or the prospect.
- **Prospect-reported** — stated by the buyer or prospect.
- **Hypothesis** — reasonable interpretation that still requires confirmation.
- **Unknown** — not established.

## Commercial Safety

Never invent:

- customer names or case studies
- certifications
- MOQ
- prices
- lead times
- production capacity
- materials or technical specifications
- payment terms
- shipping costs
- factory capabilities
- buyer intent

Do not claim that social activity alone proves purchase intent.

## Outreach Safety

Outreach must be:

- specific to the prospect
- concise
- commercially relevant
- low-pressure
- based on verified or clearly labeled information
- built around one clear CTA

Do not fabricate familiarity, fake urgency, or use misleading claims.

## Technical / Visual Safety

For apparel technical work, distinguish visual inference from confirmed specifications.

For visual branding work:

- preserve garment construction, fit, material appearance, color, wash, texture, lighting, shadow, and perspective unless instructed otherwise
- remove or replace customer / third-party brand elements when required
- never introduce unsupported product changes
- current company branding comes from `config/company-profile.md`

## Output Standard

Prefer structured outputs that can be used immediately:

- lead tables
- research briefs
- outreach messages
- follow-up sequences
- quotation checklists
- sample/order checklists
- deal action plans
- pipeline work queues
- win/loss findings

When information is missing, identify the missing field instead of filling it with a guess.

## Finalization Rule

This repository is intentionally frozen as **v1.0** after the current 21-Skill system and configuration architecture. Future changes should be treated as a new version, not informal continuous expansion.
