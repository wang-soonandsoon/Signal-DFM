# Signal-DFM

Official repository for **Signal-DFM: Roadnet-Guided Action-Token Flow Matching for Offline Traffic Signal Control**.

Signal-DFM is an offline traffic signal control framework for intelligent transportation systems. Instead of generating future traffic states and then recovering actions, Signal-DFM directly models the executable signal phase as a discrete action token. The learned discrete phase-flow score is combined with a roadnet-grounded PressLight / Max-Pressure-style pressure prior computed from CityFlow phase laneLinks.

> **Release status.** This repository is prepared as the public release entry point for the paper. The code, configuration files, and experiment scripts will be made publicly available after the paper is accepted.

## Highlights

- **Direct action-token generation:** models signal phase decisions directly over executable phase tokens.
- **Roadnet-guided pressure prior:** computes per-action pressure scores from CityFlow roadnet topology and traffic-light laneLinks.
- **Offline deployable controller:** trains from logged trajectories and evaluates frozen policies in CityFlow without additional online learning.
- **Reproducible experiments:** planned release includes training scripts, evaluation scripts, benchmark configurations, and result parsing utilities.

## Planned Repository Structure

```text
Signal-DFM/
├── README.md
├── requirements.txt
├── configs/
│   └── ...
├── data/
│   └── README.md
├── models/
│   └── ...
├── scripts/
│   └── ...
├── utils/
│   └── ...
└── docs/
    └── ...
```

The final release will include instructions for preparing the public DiffLight / CityFlow benchmark data, running Signal-DFM, reproducing the main ATT tables, and generating ablation results.

## Benchmark Protocol

Signal-DFM follows the public DiffLight benchmark protocol for CityFlow-based offline traffic signal control, including:

- CityFlow simulation environment;
- four traffic-signal phases;
- missing-observation settings such as RM and KM;
- average travel time (ATT) computed from vehicle logs;
- frozen-policy evaluation without additional online training.

## Citation

A BibTeX entry will be added after the paper is accepted.

```bibtex
@inproceedings{signaldfm2026,
  title     = {Signal-DFM: Roadnet-Guided Action-Token Flow Matching for Offline Traffic Signal Control},
  author    = {TBD},
  booktitle = {TBD},
  year      = {2026}
}
```

## License

The license will be specified when the code is released.
