# Andre Rico

**Senior Application Developer · Data systems for genomics and finance**\
Charlottesville, VA · [LinkedIn](https://linkedin.com/in/alrico) · [GitHub](https://github.com/AndreRico)

I build data systems that scale, from corporate finance data warehouses to genomic pipelines
that process billions of variants. My path runs through infrastructure, SAP and BI, FP&A, and
now bioinformatics, and the common thread is the same: take messy data from many sources and
turn it into something reliable that people can make decisions with.

> 🌐 **Prefer a website?** The same portfolio, with navigation and search:
> **[andrerico.github.io/AndreRico](https://andrerico.github.io/AndreRico/)**

---

## 📘 Writing

| Project | What it is | Stack |
| --- | --- | --- |
| [**SaaS Handbook**](writing/saas-handbook.md) | Open book on managing and operating SaaS for small teams; the repo is its own example. 📖 [Read online](https://garon-sys.github.io/saas-handbook/) | Quarto · GitHub Actions · Pages |
| **Bioinformatics** *(in progress)* | Open book on genomics and bioinformatics, built from years of notes, in the same format as the SaaS Handbook. 🗺️ [Roadmap](https://github.com/AndreRico/AndreRico/issues/1) | Quarto · GitHub Actions · Pages |

---

## 💰 Finance & data platforms

| Project | What it is | Stack |
| --- | --- | --- |
| [**12TRUE**](finance/12true.md) | Personal project: full-stack app that consolidates financial data across institutions and countries | React · TypeScript · Django · Plaid · LLMs |
| [**FP&A: area and platform**](finance/klabin-planning.md) | Built Klabin's FP&A area into the data warehouse (2016–2018), then led it full time (2018–2021): consolidation, budgeting, CAPEX, KPIs, automated books and releases, faster results | SAP BW-IP · BPC · HANA · AWS |
| [**Data warehouse & BI**](finance/klabin-bi.md) | 10 years on Klabin's SAP BI platform: one enterprise data warehouse, BW 3.5 → 7.4 on HANA, ML talent intelligence for HR, security and automation | SAP BW · HANA · ABAP · Pentaho · Hadoop/Hive |

---

## 🧬 Genomic data systems

| Project | What it is | Stack |
| --- | --- | --- |
| [**Biofilter**](bioinformatics/biofilter.md) | Persistent biological knowledge platform; its data powers the 13.8M-node knowledge graph behind DRIVE-KG | Python · SQL · ETL · CLI/API |
| [**IGEM**](bioinformatics/igem.md) | Gene–exposure knowledge base and public website for gene–environment research | Python · Docker |
| [**MyNHANES**](bioinformatics/mynhanes.md) | Downloads, normalizes and harmonizes NHANES survey data across cycles into a local database, ready for analysis | Python · Django · SQLite |
| [**Penn Medicine BioBank research**](bioinformatics/pmbb-research.md) | Statistical genetics and ML on a 260,000+ participant biobank: hearing loss, cardiology and breast cancer | Python · HPC/GPU · ML |
| [**PharmCAT**](bioinformatics/pharmcat.md) | Team member on an open-source tool that turns genotypes into prescribing recommendations; cross-platform testing and pipeline templates | Open source · VCF · cloud platforms |

---

## 📄 Publications

- Prado-Rico JM, Bargues-Carot A, …, **Rico ALG**, Hall MA, …, Huang X. [Neuron-derived circulating miRNAs reveal lead (Pb) as a key component of metal mixtures exposure](https://www.medrxiv.org/content/10.1101/2025.02.10.25322027v2). *medRxiv* (preprint), 2026.
- Rajagopalan A, Nguyen TA, Guare LA, **Rico ALG**, …, Ritchie MD, Hall MA, Romano JD, Setia-Verma S. [DRIVE-KG: Enhancing variant-phenotype association discovery in understudied complex diseases using heterogeneous knowledge graphs](https://psb.stanford.edu/psb-online/proceedings/psb26/rajagopalan.pdf). *Pacific Symposium on Biocomputing*, 2026.
- Rajagopalan A, Nguyen TA, Guare LA, **Rico ALG**, …, Setia-Verma S. [DRIVE-KG: Enhancing variant-phenotype association discovery in understudied complex diseases using heterogeneous knowledge graphs](https://www.medrxiv.org/content/10.1101/2025.08.19.25333942). *medRxiv* (preprint), 2025.
- Bargues-Carot A, Prado-Rico JM, …, **Rico ALG**, Hall MA, …, Huang X. [MicroRNA expression in asymptomatic welders: implications for biomarker discovery for environmentally-linked neurodegenerative disorders](https://www.medrxiv.org/content/10.1101/2025.02.10.25322027v1). *medRxiv* (preprint), 2025. PMID [39990579](https://pubmed.ncbi.nlm.nih.gov/39990579/).
- **Rico ALG**, Palmiero N, Ritchie MD, Hall MA. [Integrated exposomic analysis of lipid phenotypes: leveraging GE.db in environment by environment interaction studies](https://psb.stanford.edu/psb-online/proceedings/psb25/rico.pdf). *Pacific Symposium on Biocomputing*, 2025. **(first author)**
- Zhou J, **Rico ALG**, Guare L, et al. [Flexibly encoded genome-wide association study identifies novel nonadditive genetic risk variants for cardiometabolic traits](https://www.medrxiv.org/content/10.1101/2023.06.01.23290857v2). *medRxiv* (preprint), 2023.
- Zhou J, Guare L, **Rico ALG**, Gonzalez Zarzar T, Palmiero N, Assimes TL, Setia-Verma S, Hall MA. [Flexibly encoded GWAS identifies novel nonadditive SNPs in individuals of African and European ancestry](https://www.medrxiv.org/content/10.1101/2023.06.01.23290857v1.full). *medRxiv* (preprint), 2023.

---

## 🛠️ Toolbox

**Languages:** Python · TypeScript/JavaScript · SQL (T-SQL) · ABAP
**Back end & front end:** Django / DRF · REST APIs · React · Vite · Tailwind · Docker
**Data:** database design · data warehousing (SAP BW/HANA, BW-IP, BPC) · data lakes (Hadoop, Hive) · ETL (Pentaho) · Tableau
**Science & ML:** GWAS / ExWAS · gene-burden tests · ML pipelines on HPC/GPU clusters
**AI:** AI coding agents · LLM integration (document parsing, conversational assistants)
**Cloud & practices:** AWS · Linux · Agile · code review · PII protection · ADRs

→ [Career path, education and languages](about.md)

---

<sub>This repository follows the practices of the [SaaS Handbook](https://garon-sys.github.io/saas-handbook/): decisions live in [`adr/`](https://github.com/AndreRico/AndreRico/tree/main/adr), and the site is published by [GitHub Actions](https://github.com/AndreRico/AndreRico/blob/main/.github/workflows/site.yml) on every push to `main`.</sub>
