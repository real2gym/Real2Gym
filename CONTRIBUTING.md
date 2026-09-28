# Contributing to Real2Gym

Discuss the intended change in an issue or PR. Keep reconstruction, motion execution and augmentation as distinct scopes. Do not turn a scene-specific result into a general hardware or task claim.

- `skills/real2sim-prompt/SKILL.md` is the execution source of truth; references and scripts travel with the installed skill.
- Preserve the `real2sim-prompt` invocation and existing script entrypoints unless a migration is explicitly provided.
- If editing the skill entrypoint, also update the readable root `Real2Sim Prompt.md` mirror, adjusting relative reference paths.
- New validation behavior should have meaningful positive and rejection-path tests. Run `python -m unittest discover -s tests -v`.
- Keep real run evidence separate from synthetic test fixtures and illustrative artwork.
- Record dependency changes and known limits. Never repair a failing report by inventing pass flags or run provenance.
- Do not commit credentials, personal source videos, weights, private datasets, generated runs or third-party assets without suitable distribution rights.

A repository-wide license is pending owner selection. Do not assume an unstated license. PRs should state what changed, why, how it was validated, and relevant limitations.
