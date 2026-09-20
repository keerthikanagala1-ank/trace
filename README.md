# TRACE — Follow the evidence. Find the connections.

**Live:** https://kanagalakeerthi1-ank.github.io/trace/
**Alt Live:** https://kanagalakeerthi1-ank.github.io/between-the-receipts/

> A composite story assembled from the available activity records.

TRACE is MUSIC + MONEY + EVERYDAY LIFE told through receipts.

### Core Idea
**STORY → CONSTELLATION → RECEIPTS → CONNECTIONS**

The main wow moment is **RECEIPT → CONNECTIONS → STORY**.
You select a floating paper receipt → it becomes prominent → connections animate outward → you follow the trail.

> "I found a receipt. Now I can follow the trail."

### Data Used (Only Verified)
- `spotify_history.csv` - 149,860 plays
- `Daily Household Transactions.csv` - 2,461 entries

**NOT USED:** Augmented India dataset (to avoid PII)
**NOT INVENTED:** No movies, photos, messages, searches, places.

### Verified Findings Shown in Site
- 149,860 plays total
- 2,461 ledger entries
- 45,721 plays in 2015-2018
- 632 days have both music + ledger on same date
- The Beatles lead most years (2015 is different)
- Avg logged salary rises over years
- Diwali Gift ₹1,500 recurs - 2015-11-11 and 2016-10-30
- ~30% plays are midnight-5AM after IST conversion

### IST Note
All Spotify timestamps converted UTC → IST (+05:30) because ledger is INR. ~30% midnight-5AM is measured after conversion. No mood/psychological claim.

### How Connections Work
Every connection has a labeled reason:
`same date` / `same month` / `same year` / `nearby timestamp (±90m)` / `same category`

### Design
- Cinematic dark, near-black with glow
- Fonts: Instrument Serif + JetBrains Mono
- Floating paper receipts (off-white #f3efe3)
- Constellation canvas (dots = evidence, lines = same date)
- Accent colors: Ochre #ffb95c, Violet #a48cff, Green #7cffb2
- Simple top nav, 1-2s loader, custom cursor (desktop)
- Fully responsive, mobile-first

### Features
- Findings with mini-bars
- Verified timeline
- Constellation network (hover preview, click highlight)
- Receipt wall with filters: ALL / MUSIC / LEDGER / 632 OVERLAP / DIWALI ₹1500
- Detail panel with connections
- Patterns: leading artist by year, salary trend
- No backend, no build, single file

### Run
