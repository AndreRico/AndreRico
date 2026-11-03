---
title: "SaaS Handbook"
subtitle: "An open book on managing and operating software as a service for small teams"
---

**Role:** author and maintainer · 2026 – present\
**Links:** [Read online](https://garon-sys.github.io/saas-handbook/) · [Repository](https://github.com/Garon-Sys/saas-handbook) · [Portuguese edition](https://github.com/Garon-Sys/manual-saas)

## The problem

Most good material on running software in production was written for large companies. Teams of
one to eight people need method without bureaucracy: the minimum that works, with examples they
can open and copy.

## What I built

A book of 14 chapters and 4 appendices (about 10,000 words), built from the practices behind
[12TRUE](../finance/12true.md):

| Part | Topics |
| --- | --- |
| I — Management | Method, where things live, GitHub Projects, agile with iterations, documentation, people |
| II — Delivery | Code flow and PRs, the flow in VS Code, CI/CD and environments, safe migrations and feature flags |
| III — Operations | Observability, backups, incidents and postmortems, security |
| Appendices | Templates, rollout plan, reading path, glossary |

## What makes it different

- **The repository is its own example.** The chapters point to the repo's own GitHub Projects
  board, PR and issue templates, ADRs and CI workflow.
- **Security by design.** Every example uses *Farol*, a fictional SaaS, so no detail of a real
  system is exposed ([ADR 0004](https://github.com/Garon-Sys/saas-handbook/blob/main/adr/0004-fictional-case.md)).
- **Bilingual**, with one repository per edition.
- **Open licenses:** text under CC BY 4.0, code under MIT.

## Stack

Quarto · GitHub Actions · GitHub Pages · Mermaid · lychee (link checking)
