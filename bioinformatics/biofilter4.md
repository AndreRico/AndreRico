---
title: "Biofilter 4"
subtitle: "A persistent, entity-centric biological knowledge platform"
---

**Role:** developer · University of Pennsylvania, Ritchie Lab · 2024 – present\
**Links:** [Repository](https://github.com/RitchieLab/biofilter) · [Documentation](https://biofilter.readthedocs.io) · [PyPI](https://pypi.org/project/biofilter/)

## The problem

Genomic analyses keep needing the same biological knowledge: genes, variants, pathways, the
aliases each source uses, and the relationships between them. Rebuilding that integration for
every study is slow, hard to reproduce, and impossible to audit.

## What I built

Biofilter 4 is built around one idea: **build once, reuse across many analyses**.

- **Relational knowledge model:** entities, aliases, relationships and ETL metadata in one schema.
- **Resumable ETL:** each source goes through extract (raw files to staging), transform
  (normalized Parquet) and load (curated outputs into the database), with selective rollback,
  restart and cleanup.
- **Provenance:** every ETL step records source, operation, status, timestamps, hash linkage and
  errors, exposed through `biofilter etl status` and ETL reports.
- **Many ways in:** CLI, Python API (`Biofilter(...)`), SQL and notebooks, over a shared report
  layer so the CLI and the API return the same contracts.
- **Flexible deployment:** local managed database, shared team database, or a containerized app
  pointed at an external database, with the same CLI and API in all three.

## Impact

- Its data powers the **13.8M-node knowledge graph** behind DRIVE-KG
  ([medRxiv, 2025](https://www.medrxiv.org/content/10.1101/2025.08.19.25333942)).
- Published on PyPI and documented on Read the Docs.

## Stack

Python · SQL · Parquet · CLI · Docker
