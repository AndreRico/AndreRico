# ADR 0002 — Describe systems, never publish their data

- **Status:** Accepted
- **Date:** 2026-11-03

## Context

Several projects involve data that can't be public: research participants' genetic data,
unpublished results, a former employer's financial figures, and the source code of a product
under development.

## Decision

Pages describe the problem, what was built, the architecture, the stack and the scale. They never
include:

- participant-level data or unpublished study results;
- figures, reports or internal documents from Klabin or any other employer;
- schemas, addresses or infrastructure details of production systems;
- source code from 12TRUE.

Screenshots use fictional data only.

## Consequences

- Each page states what was left out, so readers know it's deliberate.
- Before adding a page, check it against this list.
