# Weekly Sales Data Review

## Project Overview

This repository contains synthetic retail sales data for a weekly reporting validation exercise.

A Data Quality Analyst has been asked to review proposed corrections to the weekly sales export before the reporting team publishes its figures.

## Objective

Assess whether the proposed corrections are accurate, supported by transaction records, and suitable for inclusion in the weekly sales report.

## Data Sources

- `sales_weekly.csv` — Current weekly sales export.
- `transaction_ledger.csv` — Supporting transaction records.
- `reporting_rules.md` — Reporting calculation and validation requirements.

## Review Scope

The review will examine:

- Duplicate and missing sales orders.
- Changes to quantities, discounts and refunds.
- Accuracy of calculated sales values.
- Differences between original and proposed figures.
- Whether unresolved discrepancies should prevent publication.

## Expected Deliverables

1. A Google Sheets validation spreadsheet containing calculations, comparisons and findings.
2. A GitHub pull request review documenting the final publish-or-hold recommendation.

## Data Privacy

All datasets in this repository are fictional and created for demonstration purposes. No real customer or company information is used.
