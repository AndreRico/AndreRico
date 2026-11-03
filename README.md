# Andre Rico

**Senior Application Developer · Bioinformatics & Data Systems**
University of Pennsylvania, Perelman School of Medicine

I build data systems that scale, from corporate finance data warehouses to genomic
pipelines that process billions of variants. My path runs through infrastructure, SAP and BI,
FP&A, and now bioinformatics, and the common thread is the same: take messy data from many
sources and turn it into something reliable that people can make decisions with.

---

## 🧬 Bioinformatics

### Biofilter 4
A persistent, entity-centric biological knowledge platform: *build once, reuse across many analyses*.
- Relational knowledge model (entities, aliases, relationships) with a resumable, provenance-tracked ETL (extract → parquet → load)
- CLI, Python API, SQL and notebook access, plus a shared report layer
- Runs as a local database, a shared team database, or a containerized app
- Its data powers the 13.8M-node knowledge graph behind DRIVE-KG

🔗 [Repository](https://github.com/RitchieLab/biofilter) · [Docs](https://biofilter.readthedocs.io) · [PyPI](https://pypi.org/project/biofilter/)

### IGEM: Integrative Genome-Exposome Method
Infrastructure and web platform for gene–environment research (geneexposure.org), with a
knowledge database (GEdb) used in exposome-wide and interaction studies. Brought AI coding
agents into the development workflow.

🔗 [Repository](https://github.com/HallLab/IGEM)

### Large-scale genomic studies
Hearing-loss and cardiology studies on biobank-scale data: rare-variant gene-burden and ExWAS
analyses, ML models on GPU clusters, and multi-terabyte pipelines designed to be replicable
across biobanks.
*(Methods and architecture only. No participant-level data is shared.)*

### PharmCAT (contributor)
Open-source pharmacogenomics tool (Stanford/Penn) that turns patient genotype files (VCF) into
drug-prescribing recommendations from CPIC, DPWG and FDA guidelines.

🔗 [pharmcat.clinpgx.org](https://pharmcat.clinpgx.org/)

### National organ/specimen-bank transaction system
Architecture and build of the SQL database behind a national specimen-bank system, deployed on
secure AWS infrastructure with Penn's cloud team.

---

## 💰 Finance & Data Platforms

### 12TRUE (personal project)
A full-stack app that consolidates financial data across institutions and countries.
- **Stack:** React · TypeScript · Vite · Tailwind · Django REST
- Bank aggregation via Plaid, US tax-reporting features (e.g. FBAR)
- LLM-based receipt parsing and a conversational assistant over the user's own financial data
- Deployed to a production server

<!-- TODO: add architecture diagram / screenshots. Source code stays private. -->

### FP&A and Business Intelligence (Klabin, 2008–2021)
Twelve-plus years building the data side of corporate finance at one of Brazil's largest
pulp-and-paper companies.
- Built the corporate budget and consolidation systems (SAP BW-IP, BPC) and an SAP HANA data platform on AWS
- Automated the managerial P&L with ETL pipelines in Pentaho, Hive and Hadoop
- Led data-warehouse development for finance, HR and operations: ABAP business rules, a predictive attrition model and the SAP BW security model

---

## 📘 SaaS Handbook

An open book on **managing and operating software as a service for small teams** (1–8 people),
built from the practices behind 12TRUE. ~10,000 words across 14 chapters and 4 appendices:
management, delivery and operations.

- **The repository is its own example:** its GitHub Projects board, PR/issue templates, ADRs and
  CI workflow are the live examples the chapters point to
- **Stack:** Quarto book, published to GitHub Pages by GitHub Actions on every merge, with a
  link-check job on every PR
- **Security by design:** every example uses *Farol*, a fictional SaaS, so no detail of a real
  system is exposed
- Bilingual: [English](https://github.com/Garon-Sys/saas-handbook) and [Portuguese](https://github.com/Garon-Sys/manual-saas) editions · text CC BY 4.0, code MIT

📖 [Read online](https://garon-sys.github.io/saas-handbook/) · 🔗 [Repository](https://github.com/Garon-Sys/saas-handbook)

---

## 📄 Selected Publications

- **Rico ALG**, et al. [Integrated exposomic analysis of lipid phenotypes: leveraging GEdb in environment-by-environment interaction studies](https://psb.stanford.edu/psb-online/proceedings/psb25/rico.pdf). *Pacific Symposium on Biocomputing*, 2025.
- [DRIVE-KG: Enhancing variant-phenotype association discovery in understudied complex diseases using heterogeneous knowledge graphs](https://www.medrxiv.org/content/10.1101/2025.08.19.25333942). *medRxiv*, 2025. (co-author)
- Flexibly encoded genome-wide association study identifies novel nonadditive genetic risk variants for cardiometabolic traits. *medRxiv*, 2023. (co-author)
- [MicroRNA expression in asymptomatic welders: implications for biomarker discovery for environmentally-linked neurodegenerative disorders](https://www.medrxiv.org/content/10.1101/2025.02.10.25322027v1). *medRxiv*, 2025. (co-author)

---

## 🛠️ Toolbox

**Languages:** Python · TypeScript/JavaScript · SQL (T-SQL) · ABAP
**Back end & front end:** Django / DRF · REST APIs · React · Vite · Tailwind · Docker
**Data:** database design · data warehousing (SAP BW/HANA, BW-IP, BPC) · data lakes (Hadoop, Hive) · ETL (Pentaho) · Tableau
**Science & ML:** GWAS / ExWAS · gene-burden tests · ML pipelines on HPC/GPU clusters
**AI:** AI coding agents · LLM integration (document parsing, conversational assistants)
**Cloud & practices:** AWS · Linux · Agile · code review · PII protection

---

## 🎓 Education
- Associate degree in Data Science (São Paulo), US-evaluated BSc equivalent
- Postgraduate degree in Business Administration, FAAP
- BSc in Accounting, Mackenzie Presbyterian University

**Languages:** Portuguese (native) · English (professional) · Spanish (reading and listening)

📫 [LinkedIn](https://linkedin.com/in/alrico)
