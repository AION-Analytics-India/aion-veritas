# AION Veritas — NIFTY, BANK NIFTY & SENSEX Pre-Open Probability Bands

[![Live bands](https://img.shields.io/badge/live%20bands-dashboard-00D4FF)](https://aionanalytics.in/veritas)
[![Validation receipts](https://img.shields.io/badge/validation-receipts-4c9)](https://aionanalytics.in/veritas/validation)
[![Model spec](https://img.shields.io/badge/model-spec-888)](https://aionanalytics.in/models/veritas)
[![Research](https://img.shields.io/badge/research-SSRN-orange)](https://papers.ssrn.com/sol3/cf_dev/AbsByAuth.cfm?per_id=7415772)

> A guiding light, not a guiding hand.

AION Veritas prepares pre-open probability bands for **NIFTY 50**, **BANK NIFTY**, and **SENSEX**. According to the **8 November 2026 scheduler audit**, the forecast is generated at **08:46 IST**, relayed at **08:47**, and checked for readiness at **08:50**; the opening-window validator runs at **09:31 IST**. These are scheduled steps, not proof of successful delivery on every trading date.

The forecast concerns the **09:15–09:30 IST opening window**, not the closing price. Public receipts document available post-session outcomes, including misses. The historical archive has publication gaps and scoring-method revisions; a single unqualified historical hit rate would be misleading.

**Current access:** a [free 7-day NIFTY 50 trial](https://aionanalytics.in/veritas)
(verified email and passkey; no card), or a paid single-/all-index subscription.
Live pre-open bands require an eligible key; the [validation archive](https://aionanalytics.in/veritas/validation) is free to read.
The [official GitHub publisher is AION-Analytics-India](https://github.com/AION-Analytics-India).

Veritas informs; it does not instruct. It describes a range to reason around, not a
call to act.

## What Veritas is

- A pre-open probability band for index-level opening-window uncertainty, subject to successful daily production and entitlement.
- An **80% design coverage target**, not an achieved coverage rate; observed performance requires dated, reproducible numerators and denominators.
- A directional assessment and reliability indication, interpreted according to the method version in use.
- Public post-session receipts for recorded dates, including misses and documented publication gaps.

## What Veritas is not

- Not a trade signal. It does not say buy or sell.
- Not a price prediction. It gives a range, not a point.
- Not investment advice. AION is not a SEBI-registered RA or IA.
- Not infallible. Misses are published publicly — that is the design, not a
  disclaimer.

## What a Veritas output conveys

A dated band may include a lower bound, upper bound, reported centre, directional assessment, direction reliability, and range confidence. The **reported model centre must not automatically be treated as the arithmetic midpoint**: field definitions and scoring rules changed during October 2026.

| Conceptual field | Meaning | Boundary |
| --- | --- | --- |
| Lower / upper band | Bounds of the forecast opening-window interval | Not buy/sell levels or a price target |
| Reported centre | Reference point defined by that method version | May differ from the arithmetic midpoint |
| Direction and reliability | Separate directional assessment that can signal uncertainty | Not a trade instruction or guaranteed result |
| Validation result | Outcome under the dated receipt's scoring contract | Compare only properly matched methodology cohorts |

This is a **conceptual field guide**, not an exact machine-readable API schema or a live subscriber band. For actual fields, consult the dated receipt or authorized service output.

## How it is scored

Range and direction are evaluated separately. The current validation job is scheduled for **09:31 IST**, after the opening window. It is not the forecast-publication time.

Historical receipt contracts are not uniform. A **13 October 2026** revision affected the reported centre and direction interpretation, and a **14 October** revision changed first-window scoring. Do not pool legacy and newer outcomes into a headline hit rate without reproducible cohort definitions and denominators.

The **80% coverage figure is a design target**, not a measured success rate. Earlier headline performance percentages were withdrawn pending reproducible, method-consistent cohort evidence; no measured accuracy rate is asserted here.

The **8 November 2026 reconciliation** identified **104 linked historical receipts**, including a previously unlinked 26 June file. It identified **56 missing calendar dates from 24 July through 17 September**, which includes non-trading days and must not be described as 56 missing trading sessions. Of the linked receipts, **66 have Day labels and 38 do not**.

**Operational limitation:** new historical API rows are not accumulating pending approval of an archival-only replacement. The current-session API still uses the 08:46 forecast snapshot. This is distinct from existing public validation receipts. Authenticated API access, signup and checkout were **not retested** in the audit.

- [How to read a band](docs/how-to-read-a-band.md)
- [How validation works](docs/validation.md)
- [Public receipt archive](https://aionanalytics.in/veritas/validation)

### Dated public example: 5 November 2026 (not a live band)

The [original public validation receipt for 5 November 2026](https://aionanalytics.in/veritas/validation/2026-11-05) records **0 of 3 ranges held**, under both its reported median-window test and its 10-of-15-minute test. It also reports **3 of 3 asserted directional assessments correct**. Range and direction are distinct outcomes; a correct direction did not prevent all three range misses.

| Index | Published lower / upper band | First-window reference reported in receipt | Minutes inside band | Asserted direction and receipt result |
| --- | --- | ---: | ---: | --- |
| NIFTY 50 | 23,988.99 / 24,288.84 | 24,354.70 | 0/15 | BULLISH, correct |
| BANK NIFTY | 55,393.68 / 56,275.54 | 56,914.45 | 0/15 | BULLISH, correct |
| SENSEX | 77,314.07 / 78,272.66 | 78,722.76 | 0/15 | BULLISH, correct |

The reference values above are the receipt's **09:15/09:20/09:25 median opening-window measures**, not closing prices or current quotes. The example predates the **5 November previous-close correction** documented by the forecaster audit. Its input provenance and applicable scoring rules must be considered before comparisons with newer cohorts. A single day, whether a miss or a hit, does **not** establish calibrated accuracy, comparative model quality, or a trading recommendation.

[Hugging Face Veritas documentation card](https://huggingface.co/aion-analytics-india/aion-veritas) is a discovery surface; it does not host the proprietary forecasting model, live band endpoint, or downloadable validation dataset. The dated website receipt remains the source for the figures in this example.

## Coverage

Three indices, at the index level only:

- NIFTY 50
- BANK NIFTY
- SENSEX

Veritas is index-level. It does not publish sector-level or single-stock bands.

## Access

Veritas offers a **free 7-day NIFTY 50 trial key** with verified email and passkey,
no card required. The trial lasts 168 hours from activation, including weekends and
market holidays. After the trial, or for BANK NIFTY and SENSEX live bands, a paid
subscription is required. The public validation receipts remain available to everyone.

For current plan prices, eligible indices and API conditions, consult the [live Veritas access page](https://aionanalytics.in/veritas) and [API catalogue](https://aionanalytics.in/apis). Billing terms are intentionally not duplicated in this documentation; the verified product catalogue is authoritative.

## Learn more

- For deeper technical readers: <https://aionanalytics.in/models/veritas>
- Public validation receipts: <https://aionanalytics.in/veritas/validation>

## Collaboration

AION builds research-led probabilistic information systems for Indian markets. For research or
engineering collaboration, contact AION Analytics (India):
<https://aionanalytics.in/>

## Identity

Published by **AION Analytics Private Limited (India)** through the official
[GitHub organization](https://github.com/AION-Analytics-India), founded by Lokesh Gupta.
[Official website](https://aionanalytics.in/) · [Product registry](https://aionanalytics.in/models).
Not affiliated with Aion Analytics LLC (United States) or AION Labs (Israel).

**Website synchronization note (8 November 2026):** the Veritas website-copy corrections were still staged at the agent's checkpoint. Live website pages may carry older schedule and performance wording until their separate release is approved and independently verified.

## Disclaimer

Content is for educational and research purposes only. It is not investment advice.
AION Analytics is not a SEBI-registered Research Analyst or Investment Adviser.
Trading involves substantial risk. SEBI regulations apply. Past performance is not
indicative of future results.