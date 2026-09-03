# Dispatch OS — Product Requirements Document

## Summary

Dispatch OS gives FMCG distributors and wholesalers a dedicated ordering platform for their retailer network, replacing phone/voice-note ordering, memory-based credit tracking, and month-end reconciliation across disconnected tools.

## Target users

- **Distributor / wholesaler admin** — manages catalog, warehouses, and credit limits, and monitors the dashboard
- **Retailer (shop owner)** — browses the catalog and places orders against their own credit line

## Problem statement

Distributors run into the same three recurring issues: orders taken by phone or voice note that get mis-heard and shipped wrong; credit exposure that lives in someone's memory rather than a system, so bad debt is only caught when a cheque bounces; and stockouts that aren't visible until retailers have already tried and failed to order.

## Functional requirements

1. **Catalog management** — load SKUs, case sizes, MOQs, and per-warehouse stock
2. **Retailer ordering** — retailers order in cases against live stock and an enforced credit limit
3. **Credit control** — per-retailer credit line; orders breaching the limit are blocked at checkout
4. **Delivery lanes** — instant restock (nearest warehouse) and standard route delivery, selectable per order
5. **Multi-warehouse** — each warehouse/dark store has its own stock and delivery radius under one account
6. **Operator dashboard** — live GMV, order queue, stock levels, and credit exposure in one view

## Out of scope (v1)

- Payment gateway integration (credit/cash recorded, not processed)
- Route/logistics optimization engine
- Retailer-side stock management

## Success metrics

- % reduction in orders lost to mis-heard/voice-note ordering and stockouts
- % reduction in bad debt as a share of the credit book
- Reduction in time spent on manual month-end reconciliation

## Status

Live at pryank18.github.io/dispatch-os/, with a tiered pricing model (Starter / Growth / Scale) already defined for go-to-market.
