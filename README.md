# shopping-list-app

Built by Veronica and Vlad - a learning project where we're both practicing full-stack development with AI integration.

## Table of Contents

- [Strategy](#strategy)
  - [User needs](#user-needs)
    - [Success metrics](#success-metrics)
    - [Product goals](#product-goals)

---

## Strategy

### User needs

- Users need to add items quickly.
- Users need items to be categorized by asiles to shop more efficiently.
- Users need recipe ingredients to shopping items automation.
- Users need reusable templates for restocking

#### Success metrics

## User Needs — Success Metrics

| Feature | Metric | Target Threshold | How to Measure |
|---|---|---|---|
| **Quick add** | Time-to-add | < 3 seconds median (open → item appears) | Manual timing during use/testing |
| | Taps required (repeat item) | 1–2 taps max | Count interaction steps |
| | Task success rate | ≥95% of test users add 5 items unaided | Usability test with a few users |
| **Aisle categorization** | Auto-categorization accuracy | ≥90% correct without manual correction | Track items needing correction vs. total |
| | Manual re-categorizations per trip | ≤1 on average | Log corrections per shopping session |
| **Recipe → shopping automation** | Ingredient parsing accuracy | ≥85% correctly extracted (name, qty, unit) with no edit | Log parse results vs. manual edits needed |
| | Merge/dedup accuracy | ≥90% of overlapping items merged correctly | Test with recipes overlapping existing list items |
| **Reusable templates** | Template reuse rate | ≥50% of new lists start from a template (once ≥2 templates exist) | Track list-creation source over time |
| | Time-to-populate from template | < 1 second perceived | Manual timing |
| | Edit rate before checkout | ≤20% of items changed/removed | Track edits per template-based list

*Note: report as "tested against X target, achieved Y."*

## Project Goals — Success Metrics

| Goal | Metric | Target / Signal | How to Measure |
|---|---|---|---|
| **Full-stack consolidation** | Concepts practiced per layer (frontend, backend, DB, deployment) | At least one concept solidified per layer, named explicitly | Session log / checklist filled in as you go |
| | Lookups vs. recall | Trending down over the course of the build | Self-log: "looked up" vs. "remembered" per session |
| | Ability to explain decisions unaided | Can explain each major decision without checking notes | Self-check at end of project |
| **Teaching (son)** | Concept explained back | ≥1 concept explained back in his own words per session | Session notes |
| | Independent engagement | He spots a bug or suggests a next step at least once | Session notes |
| | Age-appropriate accuracy | Concepts introduced without oversimplifying to the point of being wrong | Self-check per session |
| **Shipping on deadline** | Ship date met | Binary — shipped on the publicly committed date | Yes/No at deadline |
| | Scope discipline | Feature cuts logged rather than date slipping | Decision log of what was deprioritized |
| | End-to-end usability | Shipped version works fully, not a partial demo | Manual test of full user flow before ship |
| **AI integration learning** | Understanding of AI logic | Can explain what the AI is doing (not a black box) | Self-check / explain-back |
| | Error handling designed | Fallback behavior exists for AI failures/mistakes | Test deliberate bad inputs |
| | Cost/latency awareness | Know cost and speed per AI call, and the tradeoff made | Cost log per API call type |

*Note: track via a running session log rather than automated analytics.*

#### Product goals