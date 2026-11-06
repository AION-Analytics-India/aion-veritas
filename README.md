# AION Veritas — NIFTY, BANK NIFTY & SENSEX Pre-Open Probability Bands

[![Live bands](https://img.shields.io/badge/live%20bands-dashboard-00D4FF)](https://aionanalytics.in/veritas)
[![Validation receipts](https://img.shields.io/badge/validation-receipts-4c9)](https://aionanalytics.in/veritas/validation)
[![Model spec](https://img.shields.io/badge/model-spec-888)](https://aionanalytics.in/models/veritas)
[![Research](https://img.shields.io/badge/research-SSRN-orange)](https://papers.ssrn.com/sol3/cf_dev/AbsByAuth.cfm?per_id=7415772)

> A guiding light, not a guiding hand.

AION Veritas produces daily pre-open probability bands for **NIFTY 50**, **BANK NIFTY**,
and **SENSEX**. Bands are published by **08:55 IST**, ahead of the Indian market open.
The forecast covers **09:15–09:30 IST**, the first 15 minutes of the session;
historical receipts specify the exact scoring method used for each date. Results,
including misses, are published publicly after validation.

**Current access:** a [free 7-day NIFTY 50 trial](https://aionanalytics.in/veritas)
(verified email and passkey; no card), or a paid single-/all-index subscription.
Live pre-open bands require an eligible key; the [validation archive](https://aionanalytics.in/veritas/validation) is free to read.
The [official GitHub publisher is AION-Analytics-India](https://github.com/AION-Analytics-India).

Veritas informs; it does not instruct. It describes a range to reason around, not a
call to act.

## What Veritas is

- A daily probability band published before the Indian market opens.
- An 80% calibrated range — the actual open should land inside roughly 8 times out
  of 10. Past calibration does not guarantee future coverage.
- A directional lean, stated only when the model has enough conviction to assert one.
- A post-market validation receipt the same afternoon — hits and misses both on the
  public record.

## What Veritas is not

- Not a trade signal. It does not say buy or sell.
- Not a price prediction. It gives a range, not a point.
- Not investment advice. AION is not a SEBI-registered RA or IA.
- Not infallible. Misses are published publicly — that is the design, not a
  disclaimer.

## What a Veritas output looks like

Published every trading day before 08:55 IST. Each index carries a lower band, an
upper band, a midpoint, a directional lean with a confidence figure, and a range
confidence. When confidence is low, the model says so — a wide band with honest
confidence is more useful than a narrow band that hides uncertainty.

The following is an **illustrative example of the output shape only** — labelled
fields with placeholder values, not a live band and not a guarantee.

```json
{
  "index": "NIFTY 50",
  "session_date": "YYYY-MM-DD",
  "published_ist": "08:55",
  "lower_band": 23919.04,
  "upper_band": 24137.69,
  "midpoint": 24028.37,
  "directional_lean": "BEARISH",
  "directional_confidence_pct": 49.4,
  "range_confidence": "low — band is primary",
  "forecast_window_ist": "09:15-09:30"
}
```

## How it is scored

Range and direction are scored **separately**. The band is the primary product; the
directional lean is reported honestly beside it, including on days when conviction is
weak. Every session — including the ones where the band missed — is published as a
permanent, crawlable **validation receipt** that you can read before you subscribe.

- How to read a band: [`docs/how-to-read-a-band.md`](docs/how-to-read-a-band.md)
- How validation works: [`docs/validation.md`](docs/validation.md)

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

| Tier | Price | Coverage |
| --- | --- | --- |
| Single Index | ₹499 / month | One index of your choice (NIFTY 50, BANK NIFTY, or SENSEX) |
| All Indices | ₹1,999 / month | NIFTY 50 + BANK NIFTY + SENSEX |

Start the NIFTY 50 trial or subscribe: <https://aionanalytics.in/veritas> ·
Current plans and API access: <https://aionanalytics.in/apis>

## Learn more

- For deeper technical readers: <https://aionanalytics.in/models/veritas>
- Public validation receipts: <https://aionanalytics.in/veritas/validation>

## Collaboration

AION builds calibrated probabilistic models for Indian markets. For research or
engineering collaboration, contact AION Analytics (India):
<https://aionanalytics.in/>

## Identity

Published by **AION Analytics Private Limited (India)** through the official
[GitHub organization](https://github.com/AION-Analytics-India), founded by Lokesh Gupta.
[Official website](https://aionanalytics.in/) · [Product registry](https://aionanalytics.in/models).
Not affiliated with Aion Analytics LLC (United States) or AION Labs (Israel).

## Disclaimer

Content is for educational and research purposes only. It is not investment advice.
AION Analytics is not a SEBI-registered Research Analyst or Investment Adviser.
Trading involves substantial risk. SEBI regulations apply. Past performance is not
indicative of future results. 9 out of 10 retail traders lose money in options
trading.