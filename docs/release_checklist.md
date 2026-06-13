# Signal-DFM Release Checklist

This checklist records the steps required to turn this placeholder repository into the public code release after paper acceptance.

## Release Gate

- Release trigger: paper acceptance.
- Public repository: https://github.com/wang-soonandsoon/Signal-DFM
- Release target: code, configs, and scripts needed to reproduce the reported Signal-DFM experiments.

## Code To Include

- Signal-DFM model implementation.
- Roadnet-guided pressure construction from CityFlow roadnet JSON files.
- Training and evaluation entry points.
- Experiment scripts for the reported CityFlow settings.
- Result parsing utilities for ATT and unfinished-vehicle diagnostics.
- Minimal smoke tests or sanity checks for imports, shape checks, and configuration parsing.

## Code To Exclude

- Private machine paths.
- Raw large benchmark files unless redistribution is explicitly allowed.
- Generated records, logs, checkpoints, and temporary experiment outputs.
- Reviewer notes, submission drafts, or paper-internal planning files.
- Any credentials, tokens, or local environment files.

## Documentation To Include

- Environment setup.
- CityFlow installation notes.
- Public benchmark data preparation instructions.
- Commands for reproducing main results.
- Commands for reproducing ablations.
- Expected output files and metric definitions.
- Citation and license.

## Validation Before Release

- Fresh clone installs successfully.
- `python -m py_compile` passes for released Python files.
- Smoke tests run without full CityFlow training.
- A short CityFlow simulation starts successfully.
- README commands match the released paths.
- `.gitignore` excludes large artifacts and local records.

## GitHub Metadata

Recommended repository description:

```text
Code for Signal-DFM: Roadnet-Guided Action-Token Flow Matching for Offline Traffic Signal Control
```

Suggested topics:

```text
traffic-signal-control, offline-rl, flow-matching, cityflow, intelligent-transportation, max-pressure, presslight
```
