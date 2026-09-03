# Dispatch OS — Business Requirements Document

## Business objective

Replace the WhatsApp-and-notebook workflow that FMCG distributors currently use to run their retailer network with a single ordering, credit, and stock platform — reducing lost orders, bad debt, and manual reconciliation time.

## Background

Distributors typically manage retailer orders by phone or voice note, track credit exposure from memory, and reconcile sales, stock, and dues manually at month-end across notebooks and spreadsheets. This creates recurring, quantifiable losses: mis-heard orders that ship wrong and get returned, bad debt that's only caught when a cheque bounces, and stockouts that go unnoticed until retailers have already given up trying to order.

## Scope

**In scope:** retailer-facing ordering (case-based catalog), credit limit enforcement, two delivery lanes (instant/standard), multi-warehouse support, and an operator dashboard.

**Out of scope:** payment processing, logistics/route optimization, retailer-side inventory management.

## Stakeholders

- **Primary user/buyer:** distributor or wholesaler business owner/operator
- **End user:** retailer (shop owner) ordering through the platform
- **Product owner:** Pryank Wadhera

## Go-to-market model

Flat monthly subscription across three tiers (Starter, Growth, Scale), differentiated by number of retailers, warehouses, and feature access (e.g. credit aging/risk flags, full dashboard exports, API access at the top tier). Instant-lane orders carry a small per-order fee to cover dark-store logistics; standard orders carry no commission.

## Success criteria

- Reduction in orders lost to stockouts and mis-heard orders
- Reduction in bad debt as a percentage of the credit book
- Distributor onboarding (catalog load to live) achievable within one day

## Assumptions

- Distributor is willing to move retailer ordering off phone/WhatsApp onto a dedicated platform
- Retailers have basic smartphone/browser access to self-serve order

## Risks

- Adoption risk: retailers accustomed to ordering by phone may need an onboarding push to switch channels
- Credit enforcement logic must be trusted by the distributor to avoid the perception of blocking legitimate orders

## Status

Live product with defined pricing tiers; no production billing integration yet (scoped to v1 demo/prototype stage).
