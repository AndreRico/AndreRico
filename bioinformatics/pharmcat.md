---
title: "PharmCAT"
subtitle: "Team member on an open-source pharmacogenomics clinical annotation tool"
---

**Role:** team member · University of Pennsylvania · 2024 – present\
**Links:** [pharmcat.clinpgx.org](https://pharmcat.clinpgx.org/)

## What it is

PharmCAT is an open-source tool, developed by Stanford and Penn, that reads a patient's genotype
file (VCF) and turns it into drug-prescribing recommendations based on CPIC, DPWG and FDA
guidelines.

## My contribution

I was part of the PharmCAT team, with a focus on making the tool run where researchers actually
work: the cloud platforms that host the large biobank and genomic datasets.

- **Cross-platform testing.** Ran and validated PharmCAT on the main research platforms:
  - [AnVIL](https://anvilproject.org/) (NHGRI's genomic data platform)
  - [Terra](https://terra.bio/) on Google Cloud
  - [All of Us](https://www.researchallofus.org/) Researcher Workbench
  - [UK Biobank](https://www.ukbiobank.ac.uk/) Research Analysis Platform
  - [DNAnexus](https://www.dnanexus.com/)
  - [AWS](https://aws.amazon.com/)
  - and other environments
- **Pipeline templates.** Built ready-to-use pipelines for these platforms, so other researchers
  can start from a working template instead of setting PharmCAT up from scratch.

## Why it matters

Each platform has its own way of storing data, running jobs and controlling access. A tool that
works on a laptop doesn't automatically work inside a secure biobank environment. Templates that
are tested on each platform lower the barrier for any researcher who wants to turn genotype data
into pharmacogenomic insights at biobank scale.

## Stack

PharmCAT · VCF · AnVIL · Terra · All of Us · UK Biobank RAP · DNAnexus · AWS
