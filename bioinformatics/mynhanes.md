---
title: "MyNHANES"
subtitle: "A reproducible data platform for NHANES public health data"
---

**Role:** author and developer · Hall Lab · 2024 – present\
**Links:** [Repository](https://github.com/HallLab/MyNHANES) · [PyPI](https://pypi.org/project/mynhanes/)

## In one paragraph

NHANES, the US National Health and Nutrition Examination Survey, is one of the richest public
sources of health, nutrition and exposure data, collected in cycles since 1999. MyNHANES makes
it simple to use: researchers pick the data they want to analyze, download it into a local
database, and get it back normalized and harmonized across cycles, ready to feed their own
analysis pipeline.

## The problem

On the official portal, NHANES data is fragmented: one file per dataset, per cycle, each with its
own documentation page. Longitudinal analysis is the hardest part, because terms, questions and
procedures change over time. A variable can be renamed, recoded or measured differently from one
cycle to the next. Every research team ends up writing its own download, parsing and cleaning
scripts, and the transformations that make cycles comparable are rarely documented or
reproducible.

## What I built

- **Explore before downloading.** Full NHANES metadata (cycles, datasets, variables and tags) is
  searchable, so researchers choose exactly the data they want to analyze.
- **Ingestion into a local database.** The platform downloads the `.XPT` data files and `.HTM`
  documentation, parses values and metadata, and loads everything into a unified relational model
  in SQLite.
- **Normalization across cycles.** Data from every cycle lands in the same structure, so one query
  can span decades of the survey.
- **A rule-based transformation engine.** Each rule is a Python script mapped to input and output
  variables, grounded in previously published methods. Rules harmonize terms and procedures that
  changed over time and derive new variables, for example flagging participants likely to have
  Parkinson's disease from their medication records. Results are versioned and stored next to the
  raw data.
- **A simple interface to the researcher's pipeline.** Reusable queries export clean CSVs across
  cycles, ready for R, Python or Jupyter.
- **Two ways in:** a CLI (`mynhanes deploy`, `ingestion_nhanes`, `transformation`, `query`) and a
  Django Admin web interface for researchers who don't program.
- **Shared master data.** Cycles, datasets, variables, tags and rules sync from a public GitHub
  repository, so the community can contribute rules and improve variable descriptions.

## Impact

- Turns weeks of manual download and cleanup into a reproducible, logged pipeline.
- Every derived variable can be traced back to its rule and its source data.
- Published on PyPI (`pip install mynhanes`).

## Stack

Python · Django · SQLite · pandas · Dask · pyreadstat · BeautifulSoup / lxml · Poetry · pytest
