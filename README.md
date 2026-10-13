# Falcon Ridge Digital — video scripts site

Static site (no framework, no build step) with Bryce MacCabe's filming guide, the **VSL
script** and the **confirmation (post-booking) video script** for Falcon Ridge Digital's
strategy-call landing page (https://site-falcon-ridge-digital.vercel.app).

- Page: `/film-f7k2` (`film-f7k2/index.html`). `/` redirects there (`vercel.json`).
- Not indexed: `<meta name="robots" content="noindex,nofollow">`, `X-Robots-Tag: noindex, nofollow`
  on every response, and `robots.txt` → `Disallow: /`.
- Plain-text scripts: `scripts/vsl.txt`, `scripts/confirmation.txt` (same words as the page's
  "Copy script" text).

## Template

Layout, filming directions and reference photos come from the studio's standard VSL +
confirmation page (Go Rob Lacy `public/film-r8d4/`): same markup, CSS and JS; the filming
guide text is verbatim apart from client nouns; `img/ref-*.jpg` are byte-for-byte copies.
Only client-specific parts change:

- Brand: Falcon Ridge Digital's kit — Outfit (headings), DM Sans (body), Sen (labels and
  buttons); navy `#042839`, teal `#0CCCAF`, deep blue-teal `#094562`, ice `#E8F7FF`, plus
  light and dark tints. `img/emblem.svg` wraps a crop of their own logo PNG (falcon + ridge,
  not redrawn or recolored). The favicon is their FRD favicon.
- Presenter: Bryce only (solo). There are no together variants because no second presenter
  was found.
- Checklist ticks are stored in `localStorage` under `frd-film-ticks`.

## Run locally

    python3 -m http.server 8000   # then open http://localhost:8000/film-f7k2/

## Script sources (claims are Falcon Ridge Digital's own published wording)

- Founder, "Over the past 10 years, I've guided digital marketing efforts for over 1,500
  assets", Falcon Ridge Real Estate investor: https://falconridgedigital.com/conversion-launchpad-rv/
- Middleman tax, "paying for leads you should already own", data theft and race to the
  bottom on price: https://falconridgedigital.com/fundamentals/middleman-tax/
- Strategy audit, build the engine, consistent tuning, "the audit is completely free",
  modules, works with your existing management software, "You own 100% of the data",
  sister company: https://falconridgedigital.com/
- Asset-value math (−$10,000 commissions at an 8% cap rate = +$125,000) and the form fields
  used in the confirmation prep list: https://falconridgedigital.com/strategy-proposal/
- Reschedule contact: help@falconridgedigital.com · (801) 900-6025 —
  https://falconridgedigital.com/contact/

No prices, testimonials, client names, results promises or scarcity claims are used.
