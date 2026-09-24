# AGENTS.md — Layer Note project dispatcher

Layer Note は After Effects 向け CEP extension です。React + TypeScript UI、ExtendScript bridge、Vite build を持ちます。

## Governance

- Top-level contract: [`constitution/CONSTITUTION.md`](constitution/CONSTITUTION.md)
- Current Operating Model: [`organization/profiles/release-driven-solo.md`](organization/profiles/release-driven-solo.md)
- Product / architecture guidance: `README.md` and the relevant file under `docs/`

## Working rules

- Read the relevant UI / JSX / core / development / testing document before changing that surface.
- Treat the existing CEP / React / TypeScript boundaries as evidence; do not invent a replacement architecture without an explicit decision.
- Build/test/release commands must come from repository-controlled package scripts and docs rather than memory.
- Host-level After Effects verification is distinct from source-only validation and must be bound to the tested candidate.
- Never persist real credentials or machine-specific debug state in Git.
- Durable work and dependency state belongs in GitHub Issues; review/integration evidence belongs in Pull Requests.
