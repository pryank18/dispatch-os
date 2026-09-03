# Dispatch OS — Product Spec

## Problem

Distributors and wholesalers coordinate retailer orders by phone and voice note, track retailer credit from memory, and find out about stockouts only after retailers have already tried and failed to order. Sales, stock, and dues sit across notebooks and spreadsheets that don't get reconciled until month-end.

## Target user

FMCG distributors and wholesalers running one or more warehouses or dark stores, coordinating orders from a network of retail shops (kirana stores, general stores) that currently order by phone or in person.

## Goals

- Give retailers a self-serve ordering channel that doesn't depend on a salesman's visit or a phone call
- Enforce credit limits automatically at the point of order, not after
- Give the distributor one live dashboard for orders, stock, and credit exposure instead of month-end reconciliation

## Non-goals (v1)

- Payment processing beyond credit/cash order recording
- Route optimization / logistics routing engine
- Retailer-side inventory management (Dispatch OS manages the distributor's stock, not the retailer's)

## Core features (v1 scope)

| Feature | Description |
| --- | --- |
| Case-based catalog | Products priced and sold in units, cases, or bulk lots, with MOQ enforced at checkout |
| Credit limits & aging | Per-retailer credit line; orders that would breach it are blocked before placement |
| Two delivery lanes | Instant restock from the nearest warehouse, or standard route delivery on a regular schedule |
| One dashboard | Live GMV, order queue, stock levels, and credit exposure |
| Multi-warehouse | Multiple dark stores/depots under one account, each with its own stock and delivery radius |
| Retailer self-serve | Retailers can place orders any time, without waiting on a salesman's visit |

## User stories

- As a distributor, I want to load my catalog once (SKUs, case sizes, MOQs, warehouse locations) so retailers order against accurate data.
- As a distributor, I want retailer orders that would breach a credit limit blocked automatically, so bad debt isn't a visibility problem.
- As a retailer, I want to browse the catalog and place an order at any time, without waiting for a salesman's call.
- As a distributor, I want one dashboard for orders, stock, and credit exposure instead of reconciling three sources at month-end.

## Success metrics (hypothesis)

- Reduction in orders lost to mis-heard phone/voice-note orders and stockouts
- Reduction in bad debt as a share of the credit book, from enforcing limits at order time
- Reduction in month-end reconciliation time, from a live dashboard replacing manual rollups

## Status

Live — v1 is built and deployed at pryank18.github.io/dispatch-os/, including catalog, credit enforcement, dual delivery lanes, multi-warehouse support, and the operator dashboard.
