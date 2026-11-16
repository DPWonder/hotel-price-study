# Hotel prices across booking sites: 17 snapshots, September 22 to October 10, 2026

For each hotel, every booking site's nightly rate that Google Hotels listed for the same 2-night stay, reduced to a few
columns: the going rate (the price most sites agree on), the cheapest price and the site that had it, whether that
listing named a room, whether its room name matched the room at the going rate, whether fees were reported, and free
cancellation. 17 snapshots taken September 22 to October 10, 2026, with 7,044 priced hotel rows in 368 cities, plus two
files that price the same stays again a week later.

- Version 1.0.0. License: [CC BY 4.0](LICENSE). Citation: [CITATION.cff](CITATION.cff) and [below](#license-and-citation).
- Study page with the findings, charts and corrections: https://underbook.co/hotel-price-dispersion-study
- Machine-readable description of every file and column: [datapackage.json](datapackage.json) (Frictionless Data Package).
- Checksums: [SHA256SUMS](SHA256SUMS). The CSVs are byte-identical to the files served at `https://underbook.co/data/<file name>`.

## Files

All files are UTF-8 CSV with a header row, comma-separated, CRLF line endings. One row per hotel. Prices are whole US
dollars a night. Snapshot dates are UTC.

### Snapshots

| File | Snapshot | Stay (check-in to check-out) | Days ahead | Cities | Rows | Priced | Cheapest 5%+ below the going rate |
|---|---|---|---:|---:|---:|---:|---:|
| `data/hotel-price-dispersion-2026-09.csv` (r1) | 2026-09-22 | 2026-10-13 to 2026-10-15 | 21 | 25 | 426 | 424 | 331 (78.1%) |
| `data/hotel-price-dispersion-2026-09-r2.csv` (r2) | 2026-09-25 | 2026-10-30 to 2026-11-01 | 35 | 25 | 436 | 434 | 343 (79.0%) |
| `data/hotel-price-dispersion-2026-09-r3-new-cities.csv` (r3) | 2026-09-28 | 2026-11-02 to 2026-11-04 | 35 | 25 | 428 | 427 | 345 (80.8%) |
| `data/hotel-price-dispersion-2026-09-r4-new-cities.csv` (r4) | 2026-09-29 | 2026-11-03 to 2026-11-05 | 35 | 25 | 406 | 403 | 307 (76.2%) |
| `data/hotel-price-dispersion-2026-09-r5-new-cities.csv` (r5) | 2026-09-29 | 2026-11-03 to 2026-11-05 | 35 | 25 | 420 | 420 | 305 (72.6%) |
| `data/hotel-price-dispersion-2026-09-r6-us-leisure.csv` (r6) | 2026-09-29 | 2026-11-03 to 2026-11-05 | 35 | 25 | 420 | 409 | 254 (62.1%) |
| `data/hotel-price-dispersion-2026-09-r7-intl-leisure.csv` (r7) | 2026-09-29 | 2026-11-03 to 2026-11-05 | 35 | 25 | 418 | 408 | 293 (71.8%) |
| `data/hotel-price-dispersion-2026-09-r9-us-metros.csv` (r9) | 2026-09-29 | 2026-11-03 to 2026-11-05 | 35 | 24 | 399 | 397 | 243 (61.2%) |
| `data/hotel-price-dispersion-2026-09-r10-intl-cities.csv` (r10) | 2026-09-29 | 2026-11-03 to 2026-11-05 | 35 | 25 | 437 | 431 | 339 (78.7%) |
| `data/hotel-price-dispersion-2026-09-r11-us-cities.csv` (r11) | 2026-09-30 | 2026-11-04 to 2026-11-06 | 35 | 25 | 423 | 421 | 284 (67.5%) |
| `data/hotel-price-dispersion-2026-09-r12-intl-cities.csv` (r12) | 2026-09-30 | 2026-11-04 to 2026-11-06 | 35 | 25 | 430 | 427 | 332 (77.8%) |
| `data/hotel-price-dispersion-2026-09-r13-us-towns.csv` (r13) | 2026-09-30 | 2026-11-04 to 2026-11-06 | 35 | 25 | 422 | 398 | 253 (63.6%) |
| `data/hotel-price-dispersion-2026-09-r14-intl-cities.csv` (r14) | 2026-09-30 | 2026-11-04 to 2026-11-06 | 35 | 25 | 422 | 421 | 305 (72.4%) |
| `data/hotel-price-dispersion-2026-10-r15-us-cities.csv` (r15) | 2026-10-01 | 2026-11-05 to 2026-11-07 | 35 | 25 | 426 | 402 | 266 (66.2%) |
| `data/hotel-price-dispersion-2026-10-r16-intl-cities.csv` (r16) | 2026-10-01 | 2026-11-05 to 2026-11-07 | 35 | 25 | 439 | 432 | 312 (72.2%) |
| `data/hotel-price-dispersion-2026-10-r17-weekly.csv` (r17) | 2026-10-03 | 2026-11-07 to 2026-11-09 | 35 | 24 | 419 | 409 | 310 (75.8%) |
| `data/hotel-price-dispersion-2026-10-r18-weekly.csv` (r18) | 2026-10-10 | 2026-11-14 to 2026-11-16 | 35 | 23 | 394 | 381 | 292 (76.6%) |

What each snapshot covered: r1, 25 large cities in the US, Europe and Asia-Pacific; r2, the same 25 cities (a fresh
search, stays 35 days ahead); r3, r4 and r5, cities not covered before; r6, US leisure destinations; r7, international
leisure destinations; r9, smaller US metros; r10, r12, r14 and r16, international cities; r11 and r15, US cities and
towns; r13, US towns; r17 and r18, weekly snapshots, each with 10 new cities plus cities priced again with the hotels of
their earlier snapshot (same hotels, a later stay: r17 priced 14 of r2 again, r18 priced 11 of r2 and 2 of r3 again). There is no r8: that id belongs to the first week-later repeat below.

"Priced" counts rows with a going rate. "Cheapest 5%+ below the going rate" counts priced rows where
`(going_rate_usd - cheapest_usd) / going_rate_usd >= 0.05`, the rule the study's own figures use.

### Week-later repeats

| File | Stay | Priced on | Rows |
|---|---|---|---:|
| `data/hotel-price-week-later-2026-09.csv` | r1's stay, 2026-10-13 to 2026-10-15 | 2026-09-22 (r1) and 2026-09-29 | 181 |
| `data/hotel-price-week-later-r2-2026-10.csv` | r2's stay, 2026-10-30 to 2026-11-01 | 2026-09-25 (r2) and 2026-10-02 | 427 |

The same stay priced twice, seven days apart. Hotels are matched by Google's property ID and only hotels with a going
rate on both dates are included. The first repeat ran a fresh city search, so only 181 of r1's 424 priced hotels were
priced both times; the second priced r2's own hotels by their Google ID (427 of 434).

## How the prices were collected

1. **Which hotels.** For each city, Underbook asked Google Hotels for "hotels in *city*" and kept up to the first 20
   results that Google typed as a hotel (vacation rentals excluded); in practice every city has 18 rows or fewer. From
   r17 on, a search for a city outside the US includes the country ("hotels in Jaipur, India"); earlier snapshots
   searched the city name alone. A hotel returned for two cities in the same snapshot is kept once.
2. **Which prices.** Each hotel was then looked up once by its Google property ID for the snapshot's stay: 2 adults, 2
   nights, US market (`gl=us`), English, prices in US dollars. Google Hotels returns the lowest nightly rate each booking
   site lists for the hotel. Searches went through SerpApi's `google_hotels` engine on the dates in the tables above.
3. **Which price per listing.** A listing's price is its nightly rate before taxes and fees when the site reported one,
   and otherwise the nightly rate it listed, which may include them.
4. **Scoring.** Each hotel's listings were scored with the function the Underbook price check used on hotel pages:
   r2 to r18 with the rules that compare room names, introduced September 23, 2026 (r17 and r18 with that code pinned so
   they pool with r2 to r16), and r1 with the rules of September 22, 2026 (see [r1](#the-first-snapshot-r1-is-different)).
   The scoring is described column by column below.

Nothing in these files comes from a traveler: the searches were made by Underbook, and the rows hold only cities, hotel
names, booking site names, prices, flags and dates.

## Columns

### Snapshot files r2 to r18 (16 columns)

| Column | Type | Meaning |
|---|---|---|
| `city` | text | The market searched ("hotels in *city*"). Two searches priced somewhere else and are labelled for what they priced: see [Known limits](#known-limits). |
| `region` | text | Study grouping, not a standard geography: `US` (United States), `EU` (Europe, including the UK, Norway, Switzerland, Iceland and other non-EU countries), `AM` (the Americas outside the US, including Canada, Latin America, the Caribbean and Puerto Rico), `APAC` (Asia-Pacific, which in this study also holds the Middle East, Istanbul, Cape Town and Marrakech). |
| `hotel` | text | Property name as Google Hotels listed it. |
| `segment` | text | `chain` when the name matches a list of chain brand names fixed before the first run (Marriott, Hilton, Hyatt, IHG, Accor, Wyndham, Choice and others), otherwise `independent`. A name rule: a chain hotel whose name carries no brand counts as independent. |
| `sites_listed` | integer | Listing entries kept in the analysis: the 12 lowest-priced, so never more than 12 (a site listed twice counts twice). The going rate and the cheapest price use every entry, which for most hotels was more than 12. `0` when no price came back. |
| `going_rate_usd` | integer | The going rate: the nightly price shared by the largest number of listings that offer free cancellation or name a room (all listings when none do), ties broken toward the lower price. Empty when no price came back. |
| `cheapest_usd` | integer | The lowest nightly price among all listings, same basis. |
| `cheapest_site` | text | The site with the lowest price, as Google Hotels names it (for example `Booking.com`, `Expedia.ca`, `trivago DEALS`). |
| `discount_pct` | number | `100 x (going_rate_usd - cheapest_usd) / going_rate_usd`, one decimal. |
| `verdict` | text | `PARITY`: no listing more than 5% below the going rate. `UNVERIFIED_LOWER`: the cheapest listing is more than 5% below and its room is not shown to match. `REAL_LOWER_MATCHED`: the cheapest listing names a room, is more than 5% below the going rate, and its first-listed room name matches the first-listed room name of a listing priced within 2% of the going rate. Empty when no price came back. |
| `cheaper_room_name_matched` | yes/no | `yes` exactly when `verdict` is `REAL_LOWER_MATCHED`. The study page calls this the original room check. |
| `cheapest_named_a_room` | yes/no | `yes` when the cheapest listing names at least one room type, whatever its price. |
| `fees_unverified` | yes/no | `yes` when no listing for the hotel reported a before-tax rate, so every price is the rate as listed and fees such as resort fees may be missing from all of them. |
| `check_in`, `check_out` | date | The stay searched. |
| `free_cancellation_elsewhere_same_or_less` | yes/no | `yes` when, for at least one of Booking.com, Expedia, Hotels.com or Agoda (matched by name, so `Expedia.ca` counts as Expedia), that site's lowest listing has no free cancellation and another site lists free cancellation at no more than 1.02 times that price, compared on the rate including taxes and fees as the sites reported them. Empty when no price came back. |

On a row with no price (108 rows across the 16 files), the price columns, `cheapest_site`, `discount_pct`, `verdict`
and the free-cancellation flag are empty, `sites_listed` is `0`, and the other yes/no columns read `no`.

### The first snapshot (r1) is different

`data/hotel-price-dispersion-2026-09.csv` has 14 columns: no `cheaper_room_name_matched` and no
`free_cancellation_elsewhere_same_or_less`. Two columns mean something else there:

- `verdict` uses the September 22, 2026 rules: `REAL_LOWER_MATCHED` means the cheapest listing named a room and was more
  than 5% below the going rate. Rooms were **not** compared (the study's correction of September 23, 2026). A row with no
  price reads `none`.
- `cheapest_named_a_room` is `yes` only when the cheapest listing named a room **and** was more than 5% below the going
  rate: the same 45 rows as `REAL_LOWER_MATCHED`. In r2 to r18 it means only "named a room".

### Week-later files (11 columns)

`city`, `hotel`, `check_in`, `check_out` as above, then, for the first and second date (the suffix names the date,
for example `_sep22` and `_sep29`): `going_rate_usd_<date>`, `cheapest_site_<date>` and `cheaper_5pct_<date>` (`yes`
when the cheapest listing was 5% or more below the going rate that day), plus `change_pct`, the going rate's change from
the first date to the second in percent, one decimal.

## Summary figures (computed from these files)

- 7,044 priced rows in 17 snapshots. 5,114 of them (72.6%) had a cheapest price 5% or more below the going rate; per
  snapshot, 61.2% (r9) to 80.8% (r3). Median gap at those rows: 16.7% of the going rate.
- In r2 to r18, at 4,008 of the 4,783 rows with such a price (83.8%), the cheapest listing named no room.
- In r2 to r18, `cheaper_room_name_matched` is `yes` at 571 of 6,620 priced rows (8.6%).
- `fees_unverified` is `yes` at 2,136 of the 7,044 priced rows (30.3%).
- A week later, the going rate moved more than 2% at 148 of 181 hotels (first repeat) and 326 of 427 (second); the median
  change was 0.0% both times. Of the hotels with a cheaper price on the first date, 121 of 142 and 293 of 341 still had
  one on the second, with the same cheapest site at 53 and 108.

```python
import csv, glob
priced = cheaper = 0
for f in glob.glob('data/hotel-price-dispersion-*.csv'):
    for r in csv.DictReader(open(f, encoding='utf-8')):
        if r['cheapest_usd']:
            g, c = int(r['going_rate_usd']), int(r['cheapest_usd'])
            priced += 1
            cheaper += (g - c) / g >= 0.05
print(priced, cheaper)  # 7044 5114
```

These figures describe these hotels on these dates. They are not an estimate for hotels in general (see below).

## Known limits

- **One snapshot per hotel per run.** Each row is one search on one day for one stay. Prices move: in the week-later
  files the typical hotel's going rate moved about 10% either way within a week (median absolute change 10.6% and 9.0%),
  and the cheapest site changed at 101 of 181 and 285 of 427 hotels. A row says what was listed at that moment, not what
  a traveler would pay on another day.
- **Before tax versus all-in.** Prices are before taxes and fees where a site reported that figure, and the listed rate
  otherwise, so a hotel's listings can mix the two bases. `fees_unverified` flags hotels where no listing reported a
  before-tax rate. The study's hotel pages on underbook.co show the same stays all-in, so their dollar figures are higher
  than these and their discounts can differ, sometimes across the 5% line.
- **Room names are text, not rooms.** Google Hotels shows each site's lowest rate and the rooms the site names, not a
  price per room. The match compares the first-listed room name of the cheapest listing with the first-listed room names
  at the going rate, using word rules (bed types, room category, grade, shared rooms). A match is evidence, not proof, of
  the same room, and a non-match does not mean a different room: most cheaper listings name no room at all. On the
  study's own re-check of r2 to r16, 140 of the 515 hotels this column marks `yes` did not hold under a stricter
  room-name check introduced October 1, 2026, which is not in these files. In two blind rounds on samples of the
  stricter check's matches, an AI model shown only the two room names judged 42 of 50 (84%) and then 167 of 186 (90%)
  the same room (study page).
- **Which hotels and cities.** The cities were chosen by Underbook (large cities, leisure destinations, smaller US metros
  and towns), and the hotels are the first hotel results Google Hotels returned, in Google's order. Neither is a random
  sample, and the rows are not weighted by bookings or rooms. Only sites that Google Hotels listed are in the data; a
  site's "cheapest" is cheapest among what was listed that day.
- **Two searches priced somewhere else.** In r7, "hotels in Naples" (meant for Naples, Italy) returned hotels in Naples,
  Florida: they are labelled `Naples, Florida`, region `US`. In r16, "hotels in Hoi An" returned US East Coast beach
  hotels (Myrtle Beach, Virginia Beach, the Outer Banks); their 15 rows keep the label `Hoi An` with region `US`. The
  prices are real prices for real hotels. The `city` column has 369 distinct values; the study counts 368 cities because
  it does not count Hoi An.
- **Prices for visitors in other countries.** Every search asked for a traveler in the US, in US dollars, but some
  answers came back priced for a visitor elsewhere. The study page reports 34% of answers in the two October 1 snapshots
  (r15 and r16) and 31% in a separate 300-hotel test. A site that prices by country can show a US traveler a different
  price. These files do not mark which answers were affected.
- **Thresholds.** `verdict` uses "more than 5% below" (the cheapest price under 95% of the going rate), while the study's
  figures and the tables above use "5% or more below" from the two price columns. They differ on 3 rows that are exactly
  5.0% below (`PARITY` in `verdict`). `discount_pct` is rounded, so do not threshold on it: two r13 rows print `5.0` while
  the exact value is just under 5%.
- **Joining across files.** The files carry no hotel ID. The same hotel can appear in several snapshots (r2 repeats r1's
  cities with a fresh search, and the weekly snapshots price earlier hotels again: r17 priced 14 of r2 again, r18 priced 11 of r2 and 2 of r3 again), so the 7,044 rows are
  hotel-snapshots, not distinct hotels (6,478 distinct city and hotel name pairs among them). Joining on city and hotel name is approximate.
- **Lead time.** r1 priced a stay 21 days ahead; every other snapshot 35 days ahead.

Questions or corrections: hi@underbook.co. The study's corrections are listed on the study page and at
https://underbook.co/corrections.

## License and citation

The data is licensed under [Creative Commons Attribution 4.0 International](LICENSE) (CC BY 4.0). You may share and
adapt it for any purpose, including commercially, if you give credit. Please credit it as:

> Data: Underbook hotel price study, https://underbook.co/hotel-price-dispersion-study (CC BY 4.0)

To cite the dataset:

> Underbook (2026). *Hotel prices across booking sites: 17 snapshots, September 22 to October 10, 2026* (version 1.0.0)
> [Data set]. https://github.com/DPWonder/hotel-price-study

The license covers Underbook's compilation and scoring. Prices, hotel names and site names are as Google Hotels and the
booking sites listed them.

## Verify the files

```sh
shasum -a 256 -c SHA256SUMS      # macOS; on Linux: sha256sum -c SHA256SUMS
```

## Who made this

Underbook (https://underbook.co) makes a browser extension that runs this same check on a hotel page. That gives it an
interest in the question the data answers; the method, the code's rules and every correction are on the study page so
the numbers can be checked.
