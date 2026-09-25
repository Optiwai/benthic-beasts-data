# Dumbo Octopus: The 1.8 m Giant With No Traceable Source

Open data behind the distribution map and depth chart of this Benthic Beasts video.

| File | What it is |
|---|---|
| `occurrences.csv` | Every usable record of *Grimpoteuthis* retrieved from GBIF.org and OBIS on 2026-09-17 (210 records). Column `usable_mapa` = `si` marks the 154 records drawn on the map; `qc_flags` explains any exclusion |
| `gbif_datasets.csv` | GBIF datasets and number of records used from each, as registered for the GBIF derived-dataset DOI |
| `CREDITS.md` | Every source dataset, its publisher, licence and link |

## How the data were prepared

1. All occurrence records with coordinates were downloaded from the GBIF and OBIS APIs on 2026-09-17.
2. Only records whose dataset licence is **CC0 or CC BY** were kept (non-commercial, share-alike and no-derivatives licences were excluded, as were records with no licence).
3. OBIS records that duplicate a GBIF record (same coordinates to two decimals, date and rounded depth) were removed; if the two copies carried different licences, the more restrictive one applied.
4. Records were flagged, not deleted, for quality issues: placeholder or whole-degree coordinates, type-locality entries, unusually shallow depths or very wide depth ranges.

The figures on screen in the video say "retrieved September 2026": they are exactly this snapshot. GBIF and OBIS keep growing, so a new download today will give slightly different numbers.

## Citation

GBIF.org (17 September 2026) Filtered export of GBIF occurrence data https://doi.org/10.15468/dd.awrcgj

Please cite this DOI and, where possible, the individual datasets in `CREDITS.md`.
