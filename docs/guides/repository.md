# Repository organization

- Root README and Chinese overview explain Real2Gym to new users.
- `docs/guides/` holds setup, pipeline, evidence and licensing information.
- `examples/requests/` contains human-readable invocation templates.
- `assets/paper/` holds the current paper teaser and the first three method stages used in the READMEs; their source and export record is included. Earlier illustrative framework artwork and its generation provenance remain in `assets/`.
- `skills/real2sim-prompt/` remains an independently copyable skill. Its name, internal paths and v5.2 execution contracts are retained.
- `tests/` verifies evidence checks using synthetic data. CI runs those tests; it does not launch scene reconstruction.
- `docs/history/` archives earlier release narratives and obsolete illustrations. Their thresholds and iteration rules must not override current instructions.
- `Real2Sim Prompt.md` is the legacy readable mirror, not a separate implementation.

The public repository is `real2gym/Real2Gym`. Its v5.2 code and documentation are based on commit `7514e93083a40c5db0d95ae85007582f2d9a76cd` from `cskrren/Real2Gym_test`, immediately before the v5.3 update. The skill and validation contracts remain v5.2; the README adds the paper authors and current figures.

Place local runs outside the tracked source tree or in ignored `runs/`/`outputs/`. Exclude credentials, private footage, bulky meshes, model weights and generated video. Distributable assets need source and license records. A future packaged CLI or Gymnasium integration should be added only when implemented and tested.
