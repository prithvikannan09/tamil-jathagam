# Tamil Jathagam · ஜாதகம்

**Live site → https://prithvikannan09.github.io/tamil-jathagam/**

A complete Vedic Jyotisha (astrology) calculator built as a single, self-contained HTML file. No server, no dependencies, no sign-in, works offline. Birth details never leave your device.

---

## Features

- **Rasi (D1) chart** — South Indian fixed-sign format with house numbers, planet dignities, and Lagna marker
- **Navamsa (D9) chart** — divisional chart for soul strength, marriage compatibility
- **Planet positions table** — Sign, degree, house, nakshatra, pada, dignity (Exalted / Own / Mula / Debilitated)
- **Vimshottari Dasha timeline** — Mahadasha and Antardasha with exact dates; current period highlighted
- **~22 yogas, honestly evaluated** — Pancha Mahapurusha, Gajakesari, Raja, Dhana, Vipareeta Raja, Neecha Bhanga Raja, Kala Sarpa, Kemadruma, Guru-Chandala, and more — each verified for actual formation and cancellation
- **Shareable links** — birth details encoded in the URL hash; share a chart with one click
- **Print / Save as PDF** — clean print stylesheet
- **City autocomplete** — 50+ Tamil Nadu / India cities plus major global cities
- **Bilingual labels** — Tamil + English throughout

---

## Tech

Pure vanilla HTML + CSS + JavaScript — no frameworks, no build step, no API calls.

**Astronomy engine:**

| Component | Method |
|---|---|
| Sun (Earth orbit) | JPL/Standish Keplerian elements (J2000), valid 1800–2050 |
| Mercury–Saturn | Keplerian elements, geocentric conversion |
| Moon | Meeus Chapter 47 — 59 periodic terms (~1 arcminute accuracy) |
| Rahu / Ketu | True lunar node with principal periodic corrections |
| Ayanamsa | Lahiri (Chitrapaksha) — 23.8525° at J2000, 50.27"/yr drift |
| Lagna | Local Sidereal Time → Ascendant from latitude and obliquity |

---

## Verified test charts

The engine was calibrated against two known charts before any output was trusted:

**Prithvi** — 09 Dec 1992, 08:45 IST, Tiruchirappalli (10.79°N 78.70°E)
- Moon: **Rishabha / Rohini Pada 1** ✓
- Lagna: **Dhanus** ✓
- Current dasha: **Jupiter MD 2025–2041, Jupiter–Jupiter AD to ~2027** ✓

**Pushpa Amma** — 31 Jul 1962, 17:45 IST, Tirunelveli (8.71°N 77.76°E)
- Moon: **Karka / Pushya Pada 4** ✓
- Lagna: **Makara** ✓
- Current dasha: **Mars MD 2025–2032, Mars–Rahu AD 2026–27** ✓

---

## Usage

Open `index.html` in any browser, or visit the live GitHub Pages URL. Enter birth details, click **Calculate Jathagam**.

No internet connection required after first load.

---

*Built by Friday & Prithvi ✦*
