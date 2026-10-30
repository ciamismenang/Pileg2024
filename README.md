# Dashboard Suara Partai — DPRD Kabupaten Ciamis 2024

Static dashboard (no server needed): `index.html` + `data.js` + `geo.js`.

Levels: Kabupaten → Dapil → Kecamatan → Desa → RW.
Each level shows PKS votes per sub-area, the top 5 parties (PKS added if outside the top 5), and a breakdown table.
The URL changes per level (for example `#/0/2/5`), so a specific level's link can be shared.

## Publishing with GitHub Pages
1. Create a new repository on github.com (for example `dashboard-pileg-ciamis`).
2. Upload `index.html`, `data.js`, `geo.js`, and `README.md` (Add file → Upload files) → Commit.
3. Settings → Pages → Source: *Deploy from a branch* → Branch `main`, folder `/ (root)` → Save.
4. After 1–2 minutes the dashboard is at `https://<username>.github.io/dashboard-pileg-ciamis/`.

Note: GitHub Pages on a free account requires a **public** repository, so anyone with the link can open it.
The data contains only vote counts per area (no voter names).

## Data source
D.HASIL DPRD Kab. Ciamis 2024 (27 kecamatan), converted to RW using DPT weights.
Per-RW figures are estimates; desa through kabupaten totals match the official figures (740,729 valid party votes).

## Map
The map shows the winning party (or PKS strength) per dapil, kecamatan and desa.
Desa boundaries: Kemendagri administrative boundaries (2023 update), compiled in the GitHub repository Alf-Anas/batas-administrasi-indonesia; kecamatan and dapil boundaries are merged from the desa boundaries.
RW boundaries are not available, so the map stops at desa level.

## Seats
At kabupaten level the map defaults to the "Perolehan kursi" (seat allocation) view: each dot is one seat.
Seats are calculated from votes using the Sainte-Laguë method (10/7/9/8/8/8 seats for Dapil 1–6, total 50) and match the KPU Ciamis 2024 determination for all 6 dapil.
