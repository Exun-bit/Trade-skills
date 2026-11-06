# Apparel Trade Skills

A reusable personal toolkit for apparel export sales. The skills are company-agnostic and can be used across employers, factories, and brands. Current company details are maintained separately in the configuration file.

## Modules

1. **Prospecting** — identify and qualify apparel brands and potential buyers.
2. **Customer Research** — analyze a brand's products, positioning, and potential sourcing needs.
3. **Competitor Profiling** — compare apparel manufacturers using verifiable public information.
4. **Cold Email & Follow-up** — prepare personalized outreach and follow-up messages.
5. **Social Media** — plan platform-specific content for Instagram, Facebook, and LinkedIn.

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
    └── 05-social-media/SKILL.md
```
