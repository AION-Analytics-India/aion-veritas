# Validation

Veritas is published with its own scorecard. Every output — including sessions where
the band missed — is published as a permanent, crawlable **validation receipt**. You
can read the full record before you subscribe.

Public receipts: <https://dashboard.aiondashboard.site/veritas/validation>

## What a validation receipt contains

A receipt records, for a given trading day and index:

- The band that was published before the open (lower, upper, midpoint).
- The directional lean that was published, and its confidence.
- What actually happened in the opening window.
- Whether the band **held** or **broke**, and whether the directional lean was
  correct — scored **separately**.

Hits and misses are both on the record. A published miss is part of the design, not a
disclaimer.

## How a hit or miss is judged (public)

The **validation methodology is public**. A session is judged against the
**09:15–09:25 IST median opening window**:

- **Range:** the band held if the opening-window median fell inside the published
  lower–upper band; otherwise it broke.
- **Direction:** the directional lean is graded on its own, independent of whether the
  band held.

Because range and direction are judged separately, a session can hold its band while
the directional lean was weak or wrong, or vice versa. Both facts are shown.

## What is not disclosed (private)

The **prediction methodology is proprietary and patent-adjacent, and is not
disclosed**. This documentation covers only how outputs are validated and read — not
how they are produced. No features, calibration, model details, thresholds, or data
are published here or anywhere public.

## Why publish misses

Evidence first; re-validate always. A model that publishes its failures can be
checked. The validation receipts are the proof layer — read them before deciding
whether Veritas is useful to you.
