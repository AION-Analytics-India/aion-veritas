# Veritas validation and receipt coverage

Veritas publishes **post-session validation receipts** for recorded sessions, including misses. The archive is an audit trail but not a complete, method-identical daily time series. Live current-day bands require an eligible trial or subscription.

Public archive: <https://aionanalytics.in/veritas/validation>

## What a receipt documents

A dated receipt can record the pre-open lower/upper band, the reported centre, direction and reliability, observed opening-window data, and separately scored range and direction outcomes. Read exact fields and judging rules from the dated receipt or its method version rather than assuming a universal definition.

The **8 November 2026 audit** identified **104 linked receipt files**, including the previously unlinked **26 June 2026** file. **66** linked receipts carry Day labels and **38** do not. Day labels are not the authoritative receipt count or number of eligible sessions.

The archive has **56 missing calendar dates from 24 July through 17 September 2026**, between the 23 July and 18 September receipts. This count **includes non-trading days**; it is not 56 missed trading sessions.

## Scheduling and method changes

According to the 8 November scheduler audit: the forecast is generated at **08:46 IST**, relayed at **08:47**, checked for readiness at **08:50**, and the opening-window validation job runs at **09:31**. These are scheduled operations, not a guarantee of delivery or a complete daily receipt archive.

The forecast refers to the **09:15–09:30 IST opening window**. Validation criteria changed over time. The **13 October 2026** revision affected centre/direction interpretation and the **14 October** revision changed first-window candle scoring. Historical comparisons must separate incompatible cohorts, identify exact observation windows, and report dated numerators, denominators and exclusions; archived receipts must not be silently rescored.

The **80% interval-coverage figure is a design target**, not verified live coverage. Earlier approximately **72% coverage** and **84% STRONG directional accuracy** claims were not reproducible over a single comparable public cohort in the 8 November audit. They should not be represented as established results.

## Current-session versus historical API

The current-date API reads the 08:46 forecast snapshot. New historical API rows are **not presently accumulating** pending an archival-only replacement. This database persistence gap is separate from the existing public receipt files. The 8 November audit did **not** test authenticated API access, signup or checkout.

## How to interpret a validation result

- A generated forecast, successful relay, user-visible band, scored outcome and public receipt are separate states.
- Preserve misses, missing sessions, method revisions and publication gaps in any quantitative assessment.
- Score interval coverage and directional correctness separately; a weak or neutral direction does not establish a trade signal.
- Compare like-for-like date and index cohorts; do not silently pool incompatible scoring methods.
- No empirical accuracy or investment-return guarantee is asserted.

The prediction implementation remains proprietary; this public documentation describes the evidence boundary, not private feature weights, thresholds, credentials or model code. Research information only; **not investment advice**.
