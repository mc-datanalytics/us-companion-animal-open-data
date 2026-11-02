# Standardizing Shelter Breed Labels with the Vertebrate Breed Ontology (VBO)

*Published November 2026 · Open Data & Informatics*

When thousands of independent animal shelters enter intake records into disparate kennel management systems, spelling variations, colloquial mix labels, and legacy registry codes fragment national companion-animal data.

## Why Visual Breed Labeling Creates Data Drift

Shelter intake clerks routinely log animals under time pressure using visual approximations such as "Lab Mix," "Terrier Cross," or regional shorthand like "Potcake" and "catahoula cur." Without a controlled vocabulary, cross-state epidemiological studies and adoption length-of-stay benchmarks miscount mixed-ancestry dogs and domestic shorthair cats.

To make public shelter reporting reproducible, the [U.S. companion animal breed and type dataset](https://adoptanimaux.com/en/adoption/data/us/breed-types) aligns real-world shelter labels against persistent Vertebrate Breed Ontology (VBO) identifiers rather than forcing ambiguous animals into arbitrary kennel-club buckets.

## Core Normalization Layers in Open Shelter Pipelines

Reproducible crosswalk pipelines preserve raw shelter strings while attaching transparent confidence flags. Full documentation of normalization rules, coat-pattern separation, and ontology matching is published in the [AdoptAnimaux data methodology documentation](https://adoptanimaux.com/en/adoption/data/methodology).

| Raw Shelter Label | Normalized Classification | Ontology / Coat Handling |
| --- | --- | --- |
| Domestic Short Hair / Tabby | Domestic Shorthair Cat | Tabby stored separately as coat pattern |
| Black Mouth Cur / Shepherd Mix | Mixed-Breed Medium-Large Dog | Primary regional cur tag mapped with mix flag |
| Pit Bull Terrier X | Bull-Type Terrier Mix | Grouped transparently without speculative pedigree |
| Chihuahua - Long Coat | Chihuahua (Long-Haired) | Mapped to VBO breed term with coat modifier |

## Benefits for Researchers and Municipal Dashboards

- Separates true breed ancestry assertions from coat color or size descriptors such as "Tuxedo" or "Tri-color."
- Allows municipal open-data portals in Austin, Los Angeles, and New York to compare length-of-stay metrics accurately.
- Reduces breed-label stigma that historically slowed live release rates for blocky-headed mixed-breed dogs.

## References & Further Reading

- [AdoptAnimaux U.S. Breed & Type Dataset](https://adoptanimaux.com/en/adoption/data/us/breed-types) — Open reference table for U.S. shelter breed and type distributions.
- [Monarch Initiative — Vertebrate Breed Ontology](https://vbo.monarchinitiative.org/) — Community ontology for vertebrate breed classifications.
