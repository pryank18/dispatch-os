# Dispatch OS

Dispatch OS is an ordering, credit, and stock platform for FMCG distributors and wholesalers — giving each distributor their own retailer-facing ordering platform in place of phone calls, voice notes, and WhatsApp threads.

## Live demo

https://pryank18.github.io/dispatch-os/

## What it does

- **Case-based catalog** — retailers browse and order in units, cases, or bulk lots, with MOQs enforced automatically at checkout
- **Credit limits & aging** — a credit line per retailer; orders that would breach it are blocked before they're placed, not after
- **Two delivery lanes** — instant restock from the nearest warehouse, or standard route delivery on a regular schedule
- **One dashboard** — live GMV, order queue, stock levels, and credit exposure, replacing manual month-end reconciliation
- **Multi-warehouse** — several dark stores or depots under one account, each with its own stock and delivery radius
- **Retailer self-serve** — retailers can order any time, without waiting on a salesman's visit

## Product decisions

- **Block credit breaches at checkout, not after.** Today bad debt surfaces when a cheque bounces. Enforcing the limit at order time turns a collections problem into a rule.
- **Cases and MOQs as the default unit.** Retailers reorder in cases, so the catalog, pricing, and checkout are built around that rather than single units.
- **Two delivery lanes.** Instant restock from the nearest warehouse sits beside scheduled route delivery, because urgent and routine orders have different cost and speed trade-offs.
- **Record payments, don't process them.** Payment gateway, route optimization, and retailer-side inventory are out of v1 to keep the first release about ordering and credit.

**How I'd measure it:** orders lost to mis-heard voice notes and stockouts, bad debt as a share of the credit book, and hours spent on month-end reconciliation. Pricing tiers (Starter / Growth / Scale) are already defined for go-to-market.

## Documentation

- [Product spec](docs/product-spec.md)
- [PRD](docs/PRD.md)
- [BRD](docs/BRD.md)
- [MRD](docs/MRD.md)

## How it was built

Built AI-assisted with Claude as coding partner. Product scope, requirements (see `docs/`), and QA are mine.

## Status

Live — built as a self-directed product project, informed by direct field experience in distribution and logistics operations.
