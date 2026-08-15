# travels

Trip itineraries, published as self-contained HTML pages.

**Live:** https://siddharthjaswal.github.io/travels/

| Trip | Dates | Path |
|---|---|---|
| Spain | 23 Sep – 9 Oct 2026 | [`spain-2026/`](spain-2026/) |

## How these are built

Each trip is a single `index.html` with no external requests — no fonts, scripts
or styles are fetched, so a page keeps working on a phone with data off once it
has loaded. Light and dark themes both ship.

**Booking references are masked in this repo.** Airline PNRs, rail booking codes,
invoice, policy and reservation numbers are replaced with `9X••••`-style
placeholders, because a PNR plus a surname is often enough to view or change a
booking. The unmasked copies are kept locally and never committed.

## Adding a trip

1. Drop the page at `<trip-slug>/index.html`.
2. Add an entry to `TRIPS` in the index generator and rebuild `index.html`.
