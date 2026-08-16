# travels

Trip itineraries, published as self-contained HTML pages.

**Live:** https://siddharthjaswal.github.io/travels/

| Trip | Dates | Path |
|---|---|---|
| Spain | 23 Sep – 9 Oct 2026 | [`spain-2026/`](spain-2026/) |
| Adriatic Trip | 12 – 30 Aug 2025 | [`adriatic-2025/`](adriatic-2025/) |
| Milan to Bolzano | 4 – 19 Mar 2025 | [`eu-march-2025/`](eu-march-2025/) |
| Dolomites & Austria | 13 – 23 Sep 2024 | [`italo-austria-2024/`](italo-austria-2024/) |
| Barcelona to Munich | 1 – 18 Feb 2024 | [`europe-feb-2024/`](europe-feb-2024/) |
| Norway | 24 Oct – 6 Nov 2019 | [`norway-2019/`](norway-2019/) |

## How these are built

Each trip is a single `index.html` with no external requests — no fonts, scripts
or styles are fetched, so a page keeps working on a phone with data off once it
has loaded. Light and dark themes both ship, and view switching is pure CSS, so
the tabs work even where scripts are blocked.

Icons are [Lucide](https://github.com/lucide-icons/lucide) (ISC), inlined.

**Nothing private is published.** Airline PNRs, rail booking codes, invoice,
policy and reservation numbers are masked (`9X••••`), because a PNR plus a
surname is often enough to view or change a booking. Card-rewards figures are
omitted entirely, and other people's names are replaced. Unmasked copies are
kept locally and never committed.

Past trips drop the countdown, calendar export and status filters, and carry a
"Completed" badge instead.

## Adding a trip

1. Drop the page at `<trip-slug>/index.html`.
2. Add an entry to `TRIPS` in the index generator and rebuild `index.html`.
