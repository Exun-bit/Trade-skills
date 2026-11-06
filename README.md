# Apparel Trade Skills

A reusable personal toolkit for apparel export sales. The skills are company-agnostic and can be used across employers, factories, and brands. Current company details are maintained separately in configuration files.

## Architecture

The library is organized as a connected sales system rather than a collection of isolated prompts:

1. **Context** — current company profile + reusable sales context
2. **Research** — prospecting, customer research, competitor profiling, buyer personas
3. **Signals** — buying signals and lead scoring
4. **Outreach** — cold email, social media, multi-channel sequences
5. **Deal Execution** — communication, quotation, sampling, negotiation, deal coaching
6. **Operations** — Alibaba, lead management, pipeline review, analytics
7. **Learning** — win/loss analysis and feedback into future sales decisions
8. **Visual / Technical** — garment technical support and apparel visual branding

## Modules

1. Prospecting
2. Customer Research
3. Competitor Profiling
4. Cold Email & Follow-up
5. Social Media
6. Alibaba Operations
7. Customer Communication
8. Garment Technical Support
9. Lead Management
10. Apparel Visual Branding
11. Pricing & Quotation
12. Sampling & Order Execution
13. Negotiation & Objection Handling
14. Sales Analytics
15. Sales Context & ICP
16. Buying Signals
17. Outbound Sequence
18. Deal Coaching
19. Win-Loss Analysis
20. Pipeline Review
21. Sales Workflow Orchestrator

## Configuration

- `config/company-profile.md` — current employer / represented supplier. This is the only place where company-specific identity and commercial facts should live.
- `config/sales-context.md` — stable user-level sales motion, target markets, prospect types, personalization rules, and data-quality principles.

When the user changes companies, update the company profile first. Do not rewrite the skills or carry over old company facts unless explicitly confirmed.

## Core Rules

- Evidence before assumptions.
- Buying signal is separate from ICP fit.
- Verify contact data before outreach when possible.
- Never invent capabilities, certifications, customers, MOQ, lead times, prices, production capacity, or proof points.
- Separate verified facts, prospect-reported facts, hypotheses, and unknowns.
- Keep outreach concise, specific, human, and low-pressure.
- One clear CTA per outreach message.
- Do not send or perform external actions without explicit user approval.
- Preserve approved garment and product details during technical and visual work.
- Use measurable outcomes to improve the sales process.

## Workflow

```
Context / ICP
      ↓
Prospecting → Customer Research → Buying Signals
      ↓
Lead Qualification
      ↓
Cold Email / Social / Outbound Sequence
      ↓
Customer Communication
      ↓
Quotation / Sample / Technical Confirmation
      ↓
Negotiation → Deal Coaching
      ↓
Order Execution
      ↓
Lead Management → Pipeline Review → Win-Loss Analysis
      ↺
Future ICP / Outreach / Pricing improvements
```

## Repository Structure

```
.
├── README.md
├── config/
│   ├── company-profile.md
│   └── sales-context.md
└── skills/
    ├── 01-prospecting/SKILL.md
    ├── 02-customer-research/SKILL.md
    ├── 03-competitor-profiling/SKILL.md
    ├── 04-cold-email/SKILL.md
    ├── 05-social-media/SKILL.md
    ├── 06-alibaba-operations/SKILL.md
    ├── 07-customer-communication/SKILL.md
    ├── 08-garment-technical-support/SKILL.md
    ├── 09-lead-management/SKILL.md
    ├── 10-apparel-visual-branding/SKILL.md
    ├── 11-pricing-and-quotation/SKILL.md
    ├── 12-sampling-and-order-execution/SKILL.md
    ├── 13-negotiation-and-objections/SKILL.md
    ├── 14-sales-analytics/SKILL.md
    ├── 15-sales-context-and-icp/SKILL.md
    ├── 16-buying-signals/SKILL.md
    ├── 17-outbound-sequence/SKILL.md
    ├── 18-deal-coaching/SKILL.md
    ├── 19-win-loss-analysis/SKILL.md
    ├── 20-pipeline-review/SKILL.md
    └── 21-sales-workflow-orchestrator/SKILL.md
```

## External Skill Research

This library adopts general workflow ideas found in public Agent Skills repositories, while keeping the implementation original and tailored to apparel export sales. Useful patterns include shared sales context, buyer personas, signal-based prioritization, multi-channel sequencing, deal coaching, pipeline review, and win/loss feedback loops.

Referenced public projects include TheCraigHewitt sales skills, Microsoft's B2B Outreach Suite, Corey Haines' prospecting skill, and Saber Skills.

## Expansion Principle

Add a skill only when it represents a repeatable workflow that materially improves apparel export sales. Prefer improving orchestration, evidence quality, and handoffs over simply increasing the skill count.