# Alsisar Impact — Impact Monitoring Dashboard

A three-layer impact monitoring tool for [Alsisar Impact](https://www.alsisarimpact.org/), covering the Himalayan belt and Northeast India (Ladakh, Sikkim, Nagaland, Mizoram).

**Open [`index.html`](index.html) in any browser — no build step, no dependencies, fully self-contained.**

## Structure

| Layer | What it shows | Why it exists |
|---|---|---|
| **1 — Regional Overview** | Public datasets per geography: demographics, workforce, rainfall, NDVI, forest cover, hazard exposure | Establishes the operating context; the geography filter scopes the whole platform |
| **2 — Traceability & Commodity Intelligence** | A single console: provenance-layer rail (Environmental, Biodiversity, Social, Traceability, Commodity, GI Status) · schematic map of ventures → sourcing clusters · commodity record with GI status, cluster conditions, producer share and value chain. Above it, the producer's share drawn to scale; below it, the evidence base | Answers *"Where does the product come from, and can it be verified?"* |
| **3 — Portfolio Intelligence** | Dependency matrix — pick a climate shock (rainfall deficit, early frost, landslide, fire) and trace the four-step chain from hazard record → yield → ingredient shortfall → the founder's revenue line. Then the portfolio itself: farmers engaged, procurement, prices paid vs benchmarks, premiums, income uplift | Answers *"What does a bad season actually cost, and what is the venture doing differently?"* |

## Data honesty

Figures with a **dotted underline** are illustrative placeholders pending integration of venture MIS / founder-survey data. All other figures are sourced (Census 2011, ISFR 2021, GI Registry, alsisarimpact.org, LinkedIn). See [`docs/TIER1-DATA-SOURCES.md`](docs/TIER1-DATA-SOURCES.md) for the free public datasets that can replace every placeholder.

## Features

- Geography filter scopes every layer; provenance filters live in the Layer 2 rail and screen commodities by the evidence they carry
- Every chart has a table-view toggle (⊞), tooltips, and a colorblind-validated palette (adjacent-pair CVD ΔE 9.1 light / 8.4 dark)
- Editorial design system: paper ground, hairline rules, inverse ink panels, mono labelling. Light & dark themes, responsive layout
- Layer 3's cascade is computed from the Layer 1 series — the wettest three-month window, the NDVI amplitude and the hazard record all come from the same data the first layer displays
- No web fonts and no build step; the only external requests are the optional Leaflet satellite tiles in Layer 1, which degrade to a message when blocked
