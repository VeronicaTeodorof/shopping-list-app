# shopping-list-app

Built by Veronica and Vlad - a learning project where we're both practicing full-stack development with AI integration.

Target release: **Dec 18, 2026**

## Table of Contents

- [Strategy](#strategy)
  - [User needs](#user-needs)
    - [Success metrics](#success-metrics)
    - [Product goals](#product-goals)
- [Scope](#scope)
  - [User stories](#user-stories)
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

## Product Goals

1. **Reduce time and friction in building a shopping list**
   Make adding items fast enough that it doesn't feel like a chore.

2. **Make in-store shopping more efficient**
   Organize the list by aisle/category so users spend less time going back and forth through a shop, not just less time building the list beforehand.

3. **Automate the gap between "what I'm cooking" and "what I need to buy"**
   Turn a recipe directly into a usable shopping list.

4. **Support recurring/habitual shopping, not just one-off lists**
   Let users reuse past patterns (templates) instead of rebuilding the same list from scratch every week — turning the app from a single-use tool into something people keep coming back to.

---

## Scope

### User stories

**Themes**:
- Authentication
- Quick add
- Aisle categorization
- Store categorization
- Recipe-shopping automation
- Reusable templates
- UX/UI


**Authentication**

<details>
<summary>1. As a user I want to be able to register, so that I have access to all of the app's features.</summary>
</details>
<details>
<summary>2. As a user I want to be able to sign into my account and stay logged in, so that I can access my saved lists and templates without signing in repeatedly.</summary>
</details>
<details>
<summary>3. As a user I want to be able to register and sign in with a social account, for faster and easier authentication.</summary>
</details>
<details>
<summary>4. As a user I want to be able to reset my password when I forget it, so that I regain access to my account.</summary>
</details>
<details>
<summary>5. As a user I want to be able to log out, so that I can secure my account on a shared device.</summary>
</details>


**Quick add**:

<details>
<summary>6. As a user I want to add an item by typing its name, so that I can quickly build my list.</summary>
</details>
<details>
<summary>7. As a user I want to add an item with a single tap from a suggestion/autocomplete list, so that I don't have to type out items I buy often.</summary>
</details>
<details>
<summary>8. As a user I want to see previously added items suggested as I type, so that I can add them faster and avoid typos.</summary>
</details>
<details>
<summary>9. As a user I want to set a quantity for an item when adding it, so that I know how much to buy.</summary>
</details>
<details>
<summary>10. As a user I want to add multiple items at once (e.g. by pasting a list or separating with commas), so that I can quickly build a list from a note I already wrote elsewhere.</summary>
</details>
<details>
<summary>11. As a user I want to edit or delete an item after adding it, so that I can correct mistakes without starting over.</summary>
</details>
<details>
<summary>12. As a user I want to mark an item as bought/checked off while shopping, so that I can track what's left to buy.</summary>
</details>


**Aisle Categorization**:

<details>
<summary>13. As a shopper I want to create, edit and delete categories of items, so that I can keep my list organized.</summary>
</details>
<details>
<summary>14. As a shopper I want to organize my items into categories matching shop aisles, so that I can shop efficiently.</summary>
</details>
<details>
<summary>15. As an authenticated shopper I want an auto-categorization option, so that I can organize my list faster.</summary>
</details>
<details>
<summary>16. As a shopper I want to reorder my categories, so that my list follows my actual shopping route.</summary>
</details>
<details>
<summary>17. As a shopper I want to move an item from one category to another, so that I can correct a wrong categorization without deleting and re-adding it.</summary>
</details>
<details>
<summary>18. As a shopper I want to see my list grouped and displayed by category while shopping, so that I can go aisle by aisle without missing items.</summary>
</details>
<details>
<summary>19. As a authenticated shopper I want default/common categories already available when I start, so that I don't have to build a category structure from scratch.</summary>
</details>


**Store categorization**:

<details>
<summary>20. As a shopper I want to add and name the stores I shop at, so that I can organize my shopping around where I actually buy things.</summary>
</details>
<details>
<summary>21. As a shopper I want to assign items to a specific store, so that my list reflects where I actually plan to buy each thing.</summary>
</details>
<details>
<summary>22. As a shopper I want to view my list filtered by store, so that I only see what I need to buy at the store I'm currently in.</summary>
</details>
<details>
<summary>23. As a shopper I want to set the category order per store, so that my list matches that specific store's layout.</summary>
</details>
<details>
<summary>24. As a shopper I want an item without an assigned store to appear in a general/unassigned view, so that I'm not forced to pick a store for every item.</summary>
</details>


**Recipe -> Shopping Automation**:

<details>
<summary>25. As a shopper I want to input or paste a recipe's ingredient list, so that I can convert it into shopping items without typing them one by one.</summary>
</details>
<details>
<summary>26. As a shopper I want the app to extract item name, quantity and unit from each ingredient line, so that my shopping list has accurate, usable entries.</summary>
</details>
<details>
<summary>27. As a shopper I want extracted ingredients to be merged with items already on my list, so that duplicate or overlapping items are combined rather than listed twice.</summary>
</details>
<details>
<summary>28. As a shopper I want to review and edit extracted ingredients before adding them to my list, so that I can correct anything the extraction got wrong.</summary>
</details>
<details>
<summary>29. As a shopper I want extracted items to be automatically categorized, so that recipe ingredients slot into my existing category/aisle structure without extra manual work.</summary>
</details>
<details>
<summary>30. As a shopper I want to be told when an ingredient couldn't be parsed, so that I can add it manually instead of it silently disappearing.</summary>
</details>
<details>
<summary>31. As a shopper I want to save a recipe for reuse, so that I don't have to re-paste it every time I want to cook that meal again.</summary>
</details>


**Reusable Templates**:

<details>
<summary>32. As a shopper I want to save my current list as a template, so that I can reuse it for future shopping trips.</summary>
</details>
<details>
<summary>33. As a shopper I want to name and manage my templates, so that I can tell them apart and find the right one later.</summary>
</details>
<details>
<summary>34. As a shopper I want to create a new list from a template, so that I don't have to rebuild a recurring shop from scratch.</summary>
</details>
<details>
<summary>35. As a shopper I want to edit items in a list generated from a template without changing the template itself, so that a one-off change doesn't affect future trips.</summary>
</details>
<details>
<summary>36. As a shopper I want to update a template based on a completed list, so that my regular shop stays accurate as my habits change.</summary>
</details>
<details>
<summary>37. As a shopper I want to delete a template I no longer use, so that my list of templates stays relevant.</summary>
</details>


**UX/UI**:

<details>
<summary>38. As a user I want the app to be responsive across screen sizes, so that it works well on my phone, tablet, or desktop.</summary>
</details>
<details>
<summary>39. As a user I want the app to be navigable and usable with a keyboard and screen reader, so that it's accessible regardless of how I interact with it.</summary>
</details>
<details>
<summary>40. As a user I want sufficient color contrast and readable text sizing throughout the app, so that it's usable for people with visual impairments.</summary>
</details>
<details>
<summary>41. As a user I want clear, consistent navigation between sections (lists, recipes, templates, stores), so that I never feel lost in the app.</summary>
</details>
<details>
<summary>42. As a new visitor I want an attractive, welcoming landing page that explains what the app does, so that I understand its value before signing up.</summary>
</details>
<details>
<summary>43. As a user I want visual design (color, typography, spacing) to feel cohesive and intentional, so that the app feels trustworthy and polished rather than like an unfinished demo.</summary>
</details>