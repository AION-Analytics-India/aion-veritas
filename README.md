# AION Veritas — Pre-Open Probability Bands

[![Live bands](https://img.shields.io/badge/live%20bands-dashboard-00D4FF)](https://aionanalytics.in/veritas)
[![Validation receipts](https://img.shields.io/badge/validation-receipts-4c9)](https://aionanalytics.in/veritas/validation)
[![Model spec](https://img.shields.io/badge/model-spec-888)](https://aionanalytics.in/veritas-model-spec)
[![Research](https://img.shields.io/badge/research-SSRN-orange)](https://papers.ssrn.com/sol3/cf_dev/AbsByAuth.cfm?per_id=7415772)

> A guiding light, not a guiding hand.

AION Veritas is a daily pre-open probability band for **NIFTY 50**, **BANK NIFTY**,
and **SENSEX**. Each trading day the band is published by **08:55 IST**, before the
market opens, and validated publicly the same afternoon against the **09:15–09:25
median opening window**. Every session is put on the record — hits and misses alike.

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
  "validation_window_ist": "09:15-09:25 median"
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

Veritas is a paid subscription. There is no free tier. The public validation
receipts are the proof layer, not a product preview; the live forward band requires
a subscription.

| Tier | Price | Coverage |
| --- | --- | --- |
| Single Index | ₹499 / month | One index of your choice (NIFTY 50, BANK NIFTY, or SENSEX) |
| All Indices | ₹1,999 / month | NIFTY 50 + BANK NIFTY + SENSEX |

Subscribe: <https://aionanalytics.in/veritas>

## Learn more

- For deeper technical readers: <https://aionanalytics.in/models/veritas>
- Public validation receipts: <https://aionanalytics.in/veritas/validation>

## Collaboration

AION builds calibrated probabilistic models for Indian markets. For research or
engineering collaboration, contact AION Analytics (India):
<https://aionanalytics.in/>

## Identity

Founded by Lokesh Gupta. Not affiliated with Aion Analytics LLC (United States) or
AION Labs (Israel).

## Disclaimer

Content is for educational and research purposes only. It is not investment advice.
AION Analytics is not a SEBI-registered Research Analyst or Investment Adviser.
Trading involves substantial risk. SEBI regulations apply. Past performance is not
indicative of future results. 9 out of 10 retail traders lose money in options
trading.

## Website, maintainer and security contact

- Website page: https://aionanalytics.in/veritas
- Organisation: https://aionanalytics.in/ (AION Analytics, India)
- Maintainer and security contact: contact@aionanalytics.in. Report a defect through GitHub issues; report a security concern by email, not in a public issue.
- Company page: https://www.linkedin.com/company/aion-analytics-india/
