---
name: product-sourcing
description: Search, verify, and compare products, materials, components, equipment, and suppliers across Chinese and international marketplaces, distributors, and manufacturer sources. Use for product discovery, reference matching, specification filtering, supplier comparison, MOQ and lead-time review, landed-cost analysis, substitute finding, or an evidence-backed procurement shortlist. Browsing is read-only unless the user separately authorizes seller contact, quotation submission, cart changes, or purchasing.
---

# Product Sourcing

Find purchasable products or qualified suppliers that satisfy the user's technical, commercial, visual, and delivery constraints. Optimize for specification fit, total cost, evidence quality, supplier confidence, and delivery reliability rather than the largest number of links.

## Source coverage

- Chinese retail and wholesale: Taobao, Tmall, JD.com, 1688, Pinduoduo, Suning, Xianyu, and other user-named platforms.
- International retail and distribution: Amazon, Wayfair, Home Depot, Lowe's, IKEA, specialist distributors, and regional retailers.
- Direct sourcing: manufacturer sites, brand-authorized distributors, Alibaba, Made-in-China, Global Sources, and other relevant B2B directories.
- Use the user's signed-in browser when a source requires an existing login, destination-specific pricing, or image search. Use public browsing for pages that do not require that session.

Read [references/marketplace-notes.md](references/marketplace-notes.md) when platform pricing or supplier claims need interpretation. Read [references/industry-profiles.md](references/industry-profiles.md) for domain-specific compatibility and evidence checks. Use [references/comparison-schema.md](references/comparison-schema.md) for shortlist and scoring fields.

## Core boundaries

- Searching, opening listings, extracting specifications, and comparing products are read-only actions.
- Never place an order, submit payment, change a cart, add a shipping address, message a seller, request a formal quotation, or accept commercial terms without explicit user authorization for that action.
- Do not bypass CAPTCHAs, login challenges, rate limits, app-only gates, or marketplace anti-automation controls. Ask the user to complete a visible challenge when required.
- Do not treat a search-card price, crossed-out price, coupon, deposit, installment, sample price, or cheapest variant as the selected product's real price.
- Preserve exact source URLs and observation time because price, stock, specifications, seller status, and delivery estimates can change.
- For regulated, safety-critical, medical, electrical, structural, food-contact, or hazardous applications, report available documentation and gaps without certifying compliance. Recommend review by a qualified person when required.

## Build the sourcing brief

Extract or conservatively infer:

- product category, industry, end use, operating environment, quantity, and project stage;
- hard specifications, dimensions and tolerances, interfaces, materials, performance targets, compatibility, voltage, capacity, ratings, standards, and required certifications;
- visual intent, color, finish, construction, brand preference, reference images, and acceptable substitutions;
- retail, sample, prototype, or production sourcing mode; customization, OEM or ODM needs; MOQ and expected reorder volume;
- unit and total budget, preferred currency, Incoterm when relevant, and whether freight, tax, duty, tooling, or packaging is included;
- destination, required arrival date, acceptable lead time, and delivery constraints;
- acceptable sources, supplier location, used-condition policy, warranty needs, minimum seller confidence, and risk tolerance.

Ask only for missing information that would materially change the shortlist. Otherwise label conservative assumptions and proceed.

## Search and verification workflow

1. Separate hard constraints from preferences. Reject hard-constraint failures before scoring.
2. Choose the appropriate sourcing route: retail listing, authorized distributor, wholesale marketplace, direct manufacturer, OEM or ODM supplier, or a combination.
3. Search with local-language and English synonyms, technical identifiers, standards, unit variants, material names, model numbers, and common marketplace wording. Use reference-image search when relevant, then verify each result individually.
4. Open each serious candidate and verify the exact model, variant, grade, size, color, material, pack count, quantity tier, and included accessories.
5. Capture evidence using [references/comparison-schema.md](references/comparison-schema.md). Mark fields that are absent, ambiguous, image-inferred, seller-claimed, account-specific, or supported by a document.
6. For supplier sourcing, review legal or store identity, manufacturer versus trader status, years active, transaction evidence, capacity claims, MOQ, sample policy, tooling, customization, quality controls, packaging, payment terms, and references when visible.
7. Calculate known landed cost. Include selected price, quantity, mandatory accessories, tooling, samples, packaging, domestic freight, tax, duty, brokerage, international freight, and final delivery when available. Keep unknown charges separate rather than treating them as zero.
8. Separate stock, sample, production, dispatch, carrier transit, customs, and final-mile timing. Compare the combined timeline with the required arrival date.
9. Review warranty, returns, cancellation restrictions, documentation, installation, maintenance, spare parts, serviceability, and domain-specific risks from [references/industry-profiles.md](references/industry-profiles.md).
10. Rank qualifying candidates using the user's priorities. Otherwise favor hard-spec fit, evidence quality, total cost, delivery confidence, supplier confidence, support, and commercial risk in that order.
11. Reopen final candidates immediately before handoff when price, stock, or timing is important, and note any change.

## Output modes

- **Quick shortlist:** 3-5 verified products or suppliers with decisive differences.
- **Deep comparison:** 5-10 candidates, rejected options, cost analysis, risks, and recommendation.
- **Reference match:** visual or functional similarity plus specification and construction comparison.
- **Substitute finder:** alternatives for an unavailable, incompatible, late, expensive, or discontinued item.
- **Supplier shortlist:** manufacturer or distributor comparison with MOQ, sample, capacity, quality, lead-time, and commercial evidence.
- **Procurement pack:** spreadsheet-ready rows for purchasing, specification schedules, RFQs, budget tracking, samples, approvals, logistics, or installation planning.

## Handoff requirements

- Lead with the best qualifying option and explain why it wins.
- Include the exact product, variant or supplier, current price or price basis, quantity, known landed cost, lead-time evidence, warranty or returns, and clickable source URL.
- Separate confirmed facts, supplier claims, inferences, and unresolved questions.
- List hard-constraint failures under rejected options so they are not reconsidered accidentally.
- State search scope, destination assumptions, observation time, inaccessible sources, and login or CAPTCHA limitations.
- When no candidate satisfies all hard constraints, say so and present the smallest compromises rather than calling a near match compliant.
