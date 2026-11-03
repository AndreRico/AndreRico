# ADR 0001 — One repository: README as the summary, Quarto site for the details

- **Status:** Accepted
- **Date:** 2026-11-03

## Context

The portfolio has two audiences. Recruiters and engineers who land on the GitHub profile want a
one-screen summary. Others prefer a website with navigation and search. Keeping two copies of the
same content would drift.

## Decision

Keep everything in the profile repository, `AndreRico/AndreRico`:

- `README.md` is the summary and index. GitHub shows it on the profile page.
- Each project has a detail page in a subfolder (`bioinformatics/`, `finance/`, `writing/`).
- A [Quarto](https://quarto.org/) website renders the same files. Its home page includes
  `README.md`, so the summary is written once.
- GitHub Actions publishes the site to GitHub Pages on every push to `main`, the same way the
  [SaaS Handbook](https://garon-sys.github.io/saas-handbook/) does.

## Alternatives considered

- **A separate `AndreRico.github.io` repository:** a shorter URL, but the content would live in
  two places.
- **README only:** simplest, but no navigation or search for longer project pages.

## Consequences

- Detail pages are `.md`, not `.qmd`, so they also read well directly on GitHub.
- The site lives at `andrerico.github.io/AndreRico/`. It can move to the root domain later with a
  new ADR.
