# Weekly sales reporting rules (fictional)

## Reporting period

Include orders dated 2026-10-05 to 2026-10-11 (inclusive) whose payment status is `captured` in `transaction_ledger.csv`. This ledger is the reference evidence for this exercise.

## Calculation

For each order, reported net sales in GBP should equal:

`quantity × unit_price_gbp − discount_gbp − refund_gbp`

Refunds and discounts are stored as positive GBP amounts and must be subtracted once. Amounts are expressed in GBP to two decimal places. No tax or shipping is included.

## Validation controls

- Each `order_id` should appear exactly once in the final weekly export.
- Every captured order in the ledger for the period should appear in the export, and no unexplained orders should be added.
- Compare order quantity, unit price, discount and refund to the transaction ledger.
- Recalculate reported net sales for each order; any differences must be explained by independent source evidence.
- Reconcile the overall change in reported net sales to the individual order-level corrections.

## Release decision

Recommend **publish** only if there are no unresolved differences in order coverage or financial fields, and the reported values reconcile to the supporting ledger. Otherwise recommend **hold**, describe the exceptions, and state what needs further correction.

All data in this repository is synthetic.
