# AGENTS.md — Ae_LayerNote

## Governance

- Constitution: [`constitution/CONSTITUTION.md`](constitution/CONSTITUTION.md)
- Current Operating Model: [`organization/profiles/release-driven-solo.md`](organization/profiles/release-driven-solo.md)
- Project-specific architecture / build / host constraints in README and docs remain more specific authority when they preserve the Constitution.

- After Effects CEP / Vite / React / TypeScript / ExtendScript bridge architecture remains project-specific.
- existing Yarn product toolchain is not replaced by Bun; Bun is used only to run the Skills CLI.
- ZXP release and AE host validation are external/host-specific evidence bound to the tested artifact.

## Agent Skills lifecycle

- install/reconcile: `bunx skills add rebuildup/project-init --skill '*' --agent claude-code opencode codex -y`
- fresh clone: `bunx skills install`
- continuous update: `bunx skills update -p -y`
- use project scope only; global installation is not canonical
- commit CLI-generated `skills-lock.json`; do not hand-author source/hash entries
- do not modify upstream-managed project-init Skill files; keep local refinement in separate Skills/adapters/docs
