---
title: "IGEM"
subtitle: "Integrative Genome-Exposome Method: a gene–exposure knowledge base"
---

**Role:** lead developer · Penn State (Hall Lab), continued at the University of Pennsylvania · 2022 – present\
**Links:** [Repository](https://github.com/HallLab/IGEM) · [geneexposure.org](https://geneexposure.org) · [PSB 2025 paper](https://psb.stanford.edu/psb-online/proceedings/psb25/rico.pdf)

## In one paragraph

Diseases rarely come from a single gene or a single exposure. Usually they come from how genes
and the environment interact, for example how a variant changes the way the body handles a
chemical. IGEM is a platform that gathers what science already knows about genes, chemicals,
diseases, pathways and phenotypes into one knowledge base. Researchers use that knowledge to
find these interactions in their own data more reliably.

## The problem

Studying how genes and environmental exposures interact means combining genetic data with
exposure data that comes from many sources, in many formats: gene catalogs, chemical
databases, disease ontologies, pathway maps and curated literature. Each one uses different
identifiers and different file formats, and they are updated on different schedules.
Researchers had to put these together by hand for every study.

There is also a statistical problem. Testing every possible pair of variables quickly becomes
millions of tests. For example, 2,000 variants make about 2 million pairs. After correcting
for multiple testing, almost no real signal survives.

## What I built

- **A unified knowledge base (GEdb).** An ETL engine with 25 data pipelines that pulls in and
  harmonizes public biomedical sources: genes (NCBI, Ensembl, HGNC), proteins (UniProt, Pfam),
  chemicals and exposures (ChEBI, HMDB, MeSH, UniChem), curated chemical–gene and gene–disease
  links (CTD), diseases (MONDO), phenotypes (HPO), pathways (Reactome, KEGG), Gene Ontology and
  anatomy (UBERON). Everything is mapped to shared entities and relationships in a versioned
  PostgreSQL schema, with Alembic migrations and rollback-safe loads.
- **Knowledge-guided interaction filtering, the core idea.** Instead of testing every pair,
  IGEM keeps only the pairs that have a known biological link, such as a shared pathway, a
  protein interaction or a curated chemical–gene association. This can shrink the search space
  by orders of magnitude, so real signals survive multiple-testing correction, and every hit
  comes with a biological explanation.
- **A REST API and a server CLI.** The back end is built with FastAPI. It resolves identifiers
  (rsIDs, genomic coordinates, gene symbols, free-text exposure names through an NLP layer)
  and answers knowledge-base queries.
- **A Python client for researchers (`pip install igem`).** It runs the full analysis on the
  researcher's own machine: data loading, quality control, regression models, multiple-testing
  correction and plots. Only identifiers are sent to the server, never genotype or phenotype
  values. This keeps sensitive clinical data (for example NHANES-style cohorts) private.
- **A public website** ([geneexposure.org](https://geneexposure.org)) built with Next.js. It
  hosts documentation (Sphinx), downloads and a gateway to the knowledge base.
- **Deployment and operations.** Docker images, a dev/production setup on a VPS, versioned
  wheel releases and database snapshots.

## Impact

- GEdb is the knowledge base behind my first-author paper on environment-by-environment
  interaction studies ([PSB 2025](https://psb.stanford.edu/psb-online/proceedings/psb25/rico.pdf)).
- It turns a weeks-long, manual data-assembly step into a reproducible query that any lab can
  run.
- It is used by the Hall Lab's research on gene–environment interactions, first at Penn State
  and now at the University of Pennsylvania.

## Stack

Python · FastAPI · SQLAlchemy · Alembic · PostgreSQL · pandas · statsmodels · Click ·
Next.js / React · Sphinx · Docker · Linux / systemd
