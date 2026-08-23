# Product and Supplier Comparison Schema

Capture only fields supported by the task and available evidence. Do not invent missing values.

## Identity and evidence

- request or project ID, product category, industry, and end use;
- platform or source, listing title, exact URL, seller or supplier, source type, and observation time;
- exact model, selected variant, SKU, manufacturer part number, grade, or drawing revision when visible;
- evidence confidence: source-confirmed, document-supported, seller-claimed, image-inferred, calculated, or unknown.

## Technical and visual fit

- dimensions, tolerances, interfaces, capacity, performance, and hard-spec result;
- material, grade, finish, color, construction, weight, pack count, and included accessories;
- compatibility, mounting, installation, voltage, power, software or protocol support, maintenance, spare parts, and operating environment;
- standards, test reports, certifications, warranty region, and documentation gaps;
- reference-image or functional similarity and important differences.

## Commercial fields

- selected price basis, quantity, tier, MOQ, sample price, tooling or setup cost, mandatory accessories, and subtotal;
- domestic freight, packaging, tax, duty, brokerage, international shipping, final-mile delivery, and known landed total;
- Incoterm and payment terms when relevant;
- stock state, sample lead time, production lead time, dispatch estimate, transit estimate, and destination-specific arrival estimate;
- return window, return freight, warranty, customization restrictions, cancellation risk, and after-sales support.

## Supplier and decision fields

- legal or store identity, manufacturer or trader status, location, years active, rating, transaction evidence, capacity claims, quality controls, and document confidence;
- hard-constraint pass or fail with reason;
- specification fit, evidence quality, landed cost, delivery confidence, supplier confidence, support, and commercial-risk scores;
- unresolved questions, recommended verification, sample or inspection needs, and final rank.

## Default shortlist columns

| Rank | Product, variant, or supplier | Hard-spec fit | Evidence | Known landed cost | MOQ and lead time | Supplier and support | Risks or unknowns | Link |
|---|---|---|---|---|---|---|---|---|

Keep scoring explanatory. A lower-ranked candidate may be preferable when it offers stronger documentation, delivery certainty, serviceability, or easier returns.
