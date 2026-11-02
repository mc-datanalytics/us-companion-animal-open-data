# U.S. Companion Animal Adoption Listing Inventory & VBO Crosswalk Notes

Companion documentation referencing the canonical U.S. dog and cat active adoption listing inventory datasets and deterministic **Vertebrate Breed Ontology (VBO, release `releases/2026-04-15`)** source-label crosswalk maintained on **Adopt'Animaux**.

> **Methodological Guardrail:** All figures measure *active, location-ready adoption listing inventory* represented in published city hubs (not shelter intake, adoption outcomes, or unique animals). Source-label matching uses deterministic Unicode NFKC exact equality against canonical VBO labels and `EXACT` synonyms (excluding `VBO:0300020` national breed populations) across 266 source labels (190 unique exact VBO candidates covering 47,301 of 54,067 labeled listing records, 87.49%), and is explicitly not genetic breed verification.

## Canonical Datasets & Live Directories

- **[National U.S. Adoption Listing Inventory](https://adoptanimaux.com/en/adoption/data/us)** — Dated national and state listing inventory reports with downloadable CSVs ([CA](https://adoptanimaux.com/en/adoption/data/us/ca), [TX](https://adoptanimaux.com/en/adoption/data/us/tx), [FL](https://adoptanimaux.com/en/adoption/data/us/fl), [NY](https://adoptanimaux.com/en/adoption/data/us/ny), [NC](https://adoptanimaux.com/en/adoption/data/us/nc)).
- **[U.S. Source-Label to VBO Exact-Match Crosswalk](https://adoptanimaux.com/en/adoption/data/us/breed-types)** — Interactive table, CSV (`vbo-crosswalk.csv`), and JSON (`vbo-crosswalk.json`) with SHA-256 input checksums.
- **[Data Aggregation & Limitations Methodology](https://adoptanimaux.com/en/adoption/data/methodology)** — Full documentation on normalization rules and inventory caveats.
- **[Adopt'Animaux U.S. Adoption Hub](https://adoptanimaux.com/en/)** & **[U.S. Shelter & Rescue Directory](https://adoptanimaux.com/en/adoption/directory/us)** — Searchable listings for [Adoptable Dogs](https://adoptanimaux.com/en/adoption/dog), [Adoptable Cats](https://adoptanimaux.com/en/adoption/cat), and [Shelter Resources](https://adoptanimaux.com/en/associations).
