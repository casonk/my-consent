# Contributor Architecture Blueprint

This document is the starter architecture map for `my-consent`.
Keep it aligned with the real repository layout and execution flow as the repo evolves.

## Standard Architecture Assets

- PlantUML source: `docs/diagrams/repo-architecture.puml`
- Draw.io source: `docs/diagrams/repo-architecture.drawio`
- Expected renders after `archility render`:
  - `docs/diagrams/repo-architecture.puml.svg`
  - `docs/diagrams/repo-architecture.puml.png`
  - `docs/diagrams/repo-architecture.drawio.svg`
  - `docs/diagrams/repo-architecture.drawio.png`
- Shared toolchain owner: `../../util-repos/archility` from this repo

## Regeneration

```bash
cd ../../util-repos/archility
PYTHONDONTWRITEBYTECODE=1 PYTHONPATH=src python3 -m archility generate ../../doc-repos/my-consent
PYTHONDONTWRITEBYTECODE=1 PYTHONPATH=src python3 -m archility render ../../doc-repos/my-consent
```

## Current Focus Roots

- `repository root/`

## Automation

- No `.github/workflows/` directory is present yet.

## Contributor Notes

- Treat this file and the paired `docs/diagrams/` sources as the default architecture handoff surface.
- Expand this starter blueprint with repo-specific flow, dependency, and deployment details when the repository grows beyond the generated baseline.
- Update the blueprint and diagram sources together when folder structure, execution flow, or integration boundaries change.