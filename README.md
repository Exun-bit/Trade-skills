# Apparel Trade Skills

A reusable personal toolkit for apparel export sales. The skills are company-agnostic and can be used across employers, factories, and brands. Current company details are maintained separately in the configuration file.

## Modules

1. **Prospecting** — identify and qualify apparel brands and potential buyers.
2. **Customer Research** — analyze a brand's products, positioning, and potential sourcing needs.
3. **Competitor Profiling** — compare apparel manufacturers using verifiable public information.
4. **Cold Email & Follow-up** — prepare personalized outreach and follow-up messages.
5. **Social Media** — plan platform-specific content for Instagram, Facebook, and LinkedIn.
6. **Alibaba Operations** — improve product listings, keywords, storefront content, traffic, and inquiry conversion.
7. **Customer Communication** — handle buyer inquiries, quotations, negotiation, sampling, objections, complaints, and follow-up.
8. **Garment Technical Support** — interpret fabrics, construction, decoration, measurements, washes, and tech-pack terminology.
9. **Lead Management** — maintain lead records, pipeline stages, scoring, follow-ups, and reactivation.
10. **Apparel Visual Branding** — create or edit product visuals while preserving garment accuracy and handling third-party branding appropriately.
11. **Pricing & Quotation** — structure quotations, identify cost drivers, and protect commercial accuracy.
12. **Sampling & Order Execution** — control sample approval, pre-production confirmation, production checkpoints, and shipment preparation.
13. **Negotiation & Objection Handling** — diagnose buyer objections and negotiate with controlled concessions.
14. **Sales Analytics** — analyze the sales funnel, Alibaba performance, outreach response, and conversion bottlenecks.

## Company Configuration

Use `config/company-profile.md` as the single source of truth for the user's current employer or represented supplier.

When the user changes companies:
- Update the company profile using the new website and information supplied by the user.
- Re-check all company-specific claims, contacts, URLs, products, and commercial terms.
- Do not carry over the previous company's details unless the user explicitly confirms they still apply.
- Keep the skills themselves generic; do not rewrite them for each employer.

## Global Operating Rules

- Keep outreach concise, natural, personalized, and non-pushy.
- Label unknown information clearly; never invent contacts, capabilities, certifications, customers, MOQ, lead times, or production capacity.
- Separate verified facts from research hypotheses.
- Grade leads A/B/C and recommend a next follow-up date.
- Do not send messages or take external actions without the user's explicit approval.
- Use the current company profile only when a task requires company-specific information.
- Preserve the user's commercial facts when rewriting buyer messages.
- For technical questions, distinguish visual guesses from specifications that require factory or sample confirmation.
- For visual work, preserve the original garment unless the user explicitly requests a design change.
- For pricing, negotiation, and order execution, distinguish confirmed commercial terms from assumptions.
- Use measurable data when diagnosing sales or Alibaba performance.

## Typical Workflow

```
Prospecting
   ↓
Customer Research
   ↓
Lead Qualification
   ↓
Cold Email / Social Outreach
   ↓
Customer Communication
   ↓
Quotation / Sample
   ↓
Technical Confirmation
   ↓
Negotiation
   ↓
Order Execution
   ↓
Lead Management / Reorder / Reactivation
```

Alibaba Operations, Visual Branding, and Sales Analytics support the workflow throughout the process.

## Repository Structure

```
.
├── README.md
├── config/
│   └── company-profile.md
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
    └── 14-sales-analytics/SKILL.md
```

## Expansion Principle

Add new skills only when they represent a repeatable workflow that can be reused across apparel export sales tasks. Keep company-specific data in configuration rather than embedding it into skill instructions.