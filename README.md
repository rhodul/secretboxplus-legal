# secretboxplus-legal

**Status:** published. The SecretboxPlus app itself is not yet on Google Play.

Legal documents for **SecretboxPlus**, an Android app published by
Rastislav Hodul via the Google Play Store (package
`com.gnugu.secretboxplus`).

The documents here are published via GitHub Pages at:

**<https://rhodul.github.io/secretboxplus-legal/>**

## Contents

- [`privacy-policy.md`](privacy-policy.md) — rendered at
  [`/privacy-policy.html`](https://rhodul.github.io/secretboxplus-legal/privacy-policy.html).
  This is the URL registered with the Google Play Console for the App
  listing.
- [`index.md`](index.md) — minimal landing page served at the site root.

## Why a separate repo?

The SecretboxPlus application code lives in a **private** repository
(`rhodul/secretboxplus`). GitHub Pages on the free plan requires a
public repository to host pages, so this small sidecar repo exists
purely to host the legal documentation that the Play Store listing
links to.

When the App's data flows change (new SDK, new permissions, network
access, changes to backup or export behavior), the policy here must be
updated in lockstep with the App's own **Data Safety** questionnaire
answers in Play Console. The public-facing policy has a single source
of truth here; the App repo simply references this URL.

## Updating the policy

1. Edit `privacy-policy.md`.
2. Bump the **"Last updated"** line in the header to today's date.
3. Commit and push.
4. GitHub Pages rebuilds automatically in ~60 seconds.
5. Verify the rendered output loads at
   <https://rhodul.github.io/secretboxplus-legal/privacy-policy.html>.

If the change was triggered by a change to the App itself (new SDK,
etc.), the App's private repo also needs an update to the "Data
Safety" notes in `notes/plan.md` — do both in the same work session so
the public policy and the Play Console structured answers stay aligned.

## License

Copyright © 2026 Rastislav Hodul. All rights reserved.
