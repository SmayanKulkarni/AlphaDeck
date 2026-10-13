# Banking Portfolio Analytics

<!-- impeccable:product-schema 1 -->

## Platform

Power BI Desktop report, also consumable in Power BI service. This is not a web application or an iOS/Android app.

## Users

The repository supports reviewing a banking portfolio across lending, deposits, screening, acquisition cohorts and estimated fees. A specific organizational role is not confirmed.

## Product Purpose

Explore the supplied Banking.csv using the existing Power BI semantic model and native interactive visuals. Improve clarity and reduce redundant visualizations across the report.

## Capabilities and Constraints

Preserve model tables, relationships and DAX definitions. Preserve linked visuals and existing page identities; the user permits simplifying redundant visuals and reducing the primary page count. Do not present screening flags as default predictions, fee estimates as realized revenue, or current balances grouped by joining cohort as historical balances.

## Brand Commitments

The user explicitly requires a dark UI and application of Impeccable and GPT Taste.

## Evidence on Hand

Banking.csv; the original nine-page PBIX; README.md and the ten existing screenshots. The model source was extracted read-only with pbi-tools 1.2.0. The original PBIX is preserved.

## Product Principles

- Analytical meaning takes priority over decorative effects.
- Native Power BI charts and controls remain interactive.
- Cross-page filters and destinations remain coherent after consolidation.
- Existing measures are not silently redefined during a visual redesign.
