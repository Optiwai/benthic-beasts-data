# Deep-sea goosefishes (Lophiidae)

Open data behind the world map of this Benthic Beasts video ("The Anglerfish That Walks Instead of Glowing").

| File | What it is |
|---|---|
| `occurrences.csv` | Every usable record of *Lophiidae* at 200 m or deeper, retrieved from GBIF.org and OBIS on 2026-10-05 (12269 records). The map in the video draws only the 1386 records with a depth between 500 and 2,000 m (column `depth`); deeper records were left out as probable depth or trawl errors. `qc_flags` explains any other exclusion |
| `gbif_datasets.csv` | GBIF datasets and number of records used from each, as registered for the GBIF derived-dataset DOI |
| `CREDITS.md` | Every source dataset, its publisher, licence and link |

## How the data were prepared

1. All occurrence records of the family Lophiidae with coordinates and a depth of 200 m or more were downloaded from the GBIF and OBIS APIs on 2026-10-05 (most shallower records are commercial monkfish, *Lophius*).
2. Only records whose dataset licence is **CC0 or CC BY** were kept (non-commercial, share-alike and no-derivatives licences were excluded, as were records with no licence).
3. OBIS records that duplicate a GBIF record (same coordinates to two decimals, date and rounded depth) were removed; if the two copies carried different licences, the more restrictive one applied.
4. Records were flagged, not deleted, for quality issues: placeholder or whole-degree coordinates, type-locality entries, unusually shallow depths or very wide depth ranges.

The figures on screen in the video say "retrieved October 2026": they are exactly this snapshot. GBIF and OBIS keep growing, so a new download today will give slightly different numbers.

## Citation

Please cite the GBIF derived dataset DOI listed in the video description, and the individual datasets in `CREDITS.md`.
