# Tier 1 — What you can show today, with real public data

Every item below requires **no money, no partnerships, and no field data collection** — only free public datasets and transcription. Together they carry the awareness story: *the mountains are changing → farmers are leaving → the price is unfair → Alsisar's model answers it → heritage worth saving*.

| # | Point to show | How to get it |
|---|---|---|
| 1 | **Himalayan warming trend** | ERA5 / ERA5-Land temperature via [Google Earth Engine](https://earthengine.google.com/) (one short script per geography, 1990 → today). No-code alternative: cite the [ICIMOD Hindu Kush Himalaya Assessment](https://www.icimod.org/) — elevation-dependent warming faster than the global average is a published, citable headline. |
| 2 | **Snow-cover decline** | MODIS Snow Cover (`MOD10A1`, 2000–present) in Earth Engine — annual snow-days per geography. A 25-year declining line is the single most powerful "the mountains are changing" chart. |
| 3 | **Forest change** | No code needed: [Global Forest Watch](https://www.globalforestwatch.org/) exports per-state tree-cover-loss statistics (Hansen Global Forest Change) as CSV — plugs straight into Layer 1. |
| 4 | **Rainfall erraticness** | CHIRPS (1981–present) in Earth Engine — plot year-to-year variability, not just the average monthly curve. *Caveat: CHIRPS is weak in high-altitude cold desert; cross-check Ladakh against ERA5-Land.* |
| 5 | **The exodus — regional evidence** | Census of India (public): cultivator share falling decade over decade (1991 → 2001 → 2011), rural population decline in specific hill districts; plus the Uttarakhand Migration Commission's documented "ghost villages." Real, citable, and makes "communities vanish" concrete. |
| 6 | **Benchmark (mandi) prices** | [Agmarknet](https://agmarknet.gov.in/) publishes daily mandi prices; the [Spices Board](http://www.indianspices.com/) publishes large-cardamom auction prices — turns the "conventional trade" bars from illustrative to real. |
| 7 | **Wage-labor comparison** | State minimum wages and MGNREGA rates are published — "a day of wage work in Leh pays ₹X vs ₹Y from a day of farming" is buildable today, and it is the actual economics behind farmers quitting. |
| 8 | **Culture — GI register** | The [Geographical Indications Registry](https://ipindia.gov.in/gi.htm) is fully public — the Northeast holds 30+ GI tags (Raktsey Karpo apricot, Dalle Khursani, Sikkim Large Cardamom, Mizo chilli, Naga Mircha…). A real "living heritage register" panel needs only transcription in the registry's own format (application no., class, proprietor, area of production). |
| 9 | **Retail end of the price waterfall** | The ventures' own D2C listings show consumer prices — public fact; pairs with #6 to frame the farmer-share gap. |
| 10 | **Call to action** | alsisarimpact.org already has a donation page and contact — pure design work to close the story. |

## Dataset reference (from the monitoring-tool spec)

| What we measure | Source dataset | Where it lives |
|---|---|---|
| Forest gain/loss, land cover | Hansen Global Forest Change, ESA WorldCover, Dynamic World | Earth Engine catalog (all three); GFW for no-code exports |
| Rainfall | CHIRPS | Earth Engine catalog |
| Temperature & climate | ERA5 / ERA5-Land | Earth Engine catalog |
| Vegetation health | MODIS `MOD13Q1` / Sentinel-2 NDVI | Earth Engine catalog |
| Fires | MODIS / VIIRS (NASA FIRMS) | Earth Engine catalog + free near-real-time API |
| Snow & glaciers | MODIS Snow Cover `MOD10A1` | Earth Engine catalog |
| Floods & surface water | JRC Global Surface Water | Earth Engine catalog |
| Landslides | NASA Landslide Catalog + slope (Copernicus DEM) + rainfall triggers | Catalog CSV upload + Earth Engine |
| Protected areas | WDPA | Earth Engine catalog |
| Fragile / important zones | Key Biodiversity Areas | Request free from BirdLife International → QGIS → GeoJSON |
| Threatened species overlap | IUCN Red List range maps | Request from IUCN → QGIS overlay |

**Tier 2 (label as indicative until surveyed):** conventional-trade farm-gate prices, crop-area decline series, engagement-growth trajectory.
**Tier 3 (founder survey only — KoboToolbox/ODK):** retention ("farmers who stayed"), youth returning, actual prices paid, hectares kept under traditional crops, testimonies.
