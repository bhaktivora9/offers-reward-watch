---
doc: scope
status: approved
---

# OfferWatch

An API-first service that collects public US rewards and merchant offers and turns them into structured, source-backed records.

## The Unique Kernel
OfferWatch uses AI to pull buried offer details into consistent records while keeping each detail traceable to its source. It marks unpublished information, such as an expiration date, as unknown instead of guessing, and a failure at one source does not prevent results from the others.

## Who It's For
People who regularly check promotions and developers building rewards or personal-finance apps who need current offer data in a usable format. Today, they manually check merchant websites, read fine print themselves, or maintain separate scrapers for each source.

## The Core Loop
A user opens a simple dashboard, clicks **Refresh offers**, and OfferWatch gathers offers from a small set of public websites. It normalizes the results into readable records and lets the user inspect each offer's supporting source text.

## Inspiration & Identity
The experience should make offer information consistent, readable, and easy to verify. A more specific visual direction has not been established.

## Why This Matters to the Learner
The learner wants to test whether AI can reliably turn live web content into useful structured data, with evidence for extracted details and honest handling of uncertainty and source failures.

## What "Working" Looks Like
A demonstrable end-to-end refresh collects offers from two or three public websites and makes normalized records available through the dashboard and an API. A record includes the merchant, benefit, conditions such as minimum spend, exclusions, and activation requirements, expiration when published (otherwise unknown), source link, and collection time; its supporting source text can be inspected. If one site fails, results from the others remain available and the failure is visible.

## The POC Boundary
Include one complete collection workflow for two or three publicly available US offer sources, AI-assisted extraction and normalization, a developer-consumable API, and a simple dashboard for demonstrating and inspecting refresh results. Keep results traceable to source text and do not infer unpublished details.

## Later
- Compare refreshes to highlight changed offers.
- Expand the number of supported sources.
- Consider personalized bank offers, eligibility matching, card recommendations, payment routing, and external partner API integrations after the public-source collection workflow is proven.

## Explicitly Cut
- Personalized bank offers, eligibility matching, card recommendations, payment routing, and external partner API integrations are outside this proof of concept; they do not prove the core public-source extraction and API workflow.
