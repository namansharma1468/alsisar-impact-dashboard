# Alsisar Impact — Impact Monitoring Dashboard

A three-layer impact monitoring tool for [Alsisar Impact](https://www.alsisarimpact.org/), covering the Himalayan belt and Northeast India (Ladakh, Sikkim, Nagaland, Mizoram).

**Open [`index.html`](index.html) in any browser — no build step, no dependencies, fully self-contained.**

## Structure

| Layer | What it shows | Why it exists |
|---|---|---|
| **1 — Regional Overview** | Public datasets per geography: demographics, workforce, rainfall, NDVI, forest cover, hazard exposure | Establishes the operating context; the geography filter scopes the whole platform |
| **2 — Traceability & Commodity Intelligence** | Sourcing map, provenance filters (Environmental, Biodiversity, Social, Traceability, Commodity, GI Status), commodity profiles, GI records, farmer share, value chains | Answers *"Where does the product come from, and can it be verified?"* |
| **3 — Portfolio Intelligence** | Venture-level overlay: farmers engaged, procurement, prices paid vs benchmarks, premiums, income uplift | Answers *"What is the venture doing differently?"* |

## Data honesty

Figures with a **dotted underline** are illustrative placeholders pending integration of venture MIS / founder-survey data. All other figures are sourced (Census 2011, ISFR 2021, GI Registry, alsisarimpact.org, LinkedIn). See [`docs/TIER1-DATA-SOURCES.md`](docs/TIER1-DATA-SOURCES.md) for the free public datasets that can replace every placeholder.

## Features

- Geography filter (all layers) and provenance filters (Layer 2)
- Every chart has a table-view toggle (⊞), tooltips, and a colorblind-validated palette
- Light & dark themes, responsive layout
- Zero external requests — works offline and inside strict-CSP hosts
