---
name: apparel-sales-workflow-orchestrator
description: Select and chain the apparel trade skills needed for a task, preserving context and preventing duplicate work.
---

# Sales Workflow Orchestrator

## Objective
Act as the routing layer for the skill library. Select the smallest useful chain of skills for the user's task and preserve outputs between steps.

## Routing
### New Prospect
Use: 01 Prospecting → 02 Customer Research → 16 Buying Signals → 04 Cold Email or 17 Outbound Sequence → 09 Lead Management

### Targeted Brand Development
Use: 02 Customer Research → 16 Buying Signals → 17 Outbound Sequence

### Existing Buyer Conversation
Use: 07 Customer Communication → 18 Deal Coaching → 09 Lead Management

### Price Request
Use: 08 Garment Technical Support → 11 Pricing & Quotation → 13 Negotiation if needed → 09 Lead Management

### Sample Development
Use: 08 Garment Technical Support → 12 Sampling & Order Execution → 07 Customer Communication

### Active Deal
Use: 18 Deal Coaching → 13 Negotiation if needed → 12 Sampling & Order Execution → 09 Lead Management

### Alibaba Product Optimization
Use: 06 Alibaba Operations → 14 Sales Analytics

### Sales Performance Review
Use: 09 Lead Management → 14 Sales Analytics → 20 Pipeline Review → 19 Win-Loss Analysis

### Company Change
Update config/company-profile.md first, then re-check all company-specific claims before using outreach or marketing skills.

## Execution Rules
- Do not run every skill for every task.
- Reuse already verified research instead of repeating it.
- Pass evidence and unknowns between skills.
- If a required input is missing, ask only for the minimum information needed.
- Never perform external sending or account changes without explicit approval.
- Keep company-specific facts in configuration, not in the skill instructions.