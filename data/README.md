# Data files for "Wild Country" (FIT3179 DV2)

Built 14 Oct 2026. Every number is copied from the source named below, except where a column says "approximate".

| File | Source | Notes |
|---|---|---|
| states.csv | DCCEEW CAPAD 2024 (30 Jun 2024), Jurisdiction sheet; ABS National, state and territory population, March 2026 (released 17 Sep 2026) | people_per_km2_protected, population_share_pct and tile positions are calculated here |
| waffle.csv | CAPAD 2024, Type sheet (% of Australia) | 1 square = 0.5% of Australia. "National parks" = the five CAPAD national park types |
| parks.csv | CAPAD 2024 protected-area layer (ArcGIS REST service, layer 0), national park types only | One row per park per state; polygon parts summed; type_group = the park type covering most of the area; coordinates are the largest part's centroid. Reconciles with the CAPAD Type sheet to 0.008% |
| bioregions.csv, bioregion_iucn.csv | CAPAD 2024, IBRA Bioregions and Bioregion by IUCN sheets | 89 regions; Coral Sea and Subantarctic Islands are protected under marine reserves (land_region = no). Added by me for the charts: land_rank (1 = least protected of the 87 land regions) and display_group (the 12 least and 8 most protected) |
| visits.csv | NSW NPWS park visitor survey 2024/25; Tasmania PWS Visitors to Selected Parks and Reserves 2020-21 to 2025-26; Parks Australia / Director of National Parks annual reports 2022-23 and 2024-25 | Counting methods differ by agency (see method_note). Do not rank across agencies. Tasmania coordinates are APPROXIMATE |
| nsw_total_visits.csv | NSW NPWS park visitor survey | 2022 adult + child differs from the published total by 158,025; 2018 by 1. Check the source |
| australia_states.geojson | GitHub: rowanhogan/australian-states | Original ABS edition and licence unconfirmed. Outlines are approximate: each state's area is within 1.1% of the official figure (largest gap: SA). Simplified to about 200 m and snapped to 4 decimals (areas unchanged, all outlines valid); Lord Howe Island removed for display |
