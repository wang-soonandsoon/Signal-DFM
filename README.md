# Signal-DFM

Official repository for **Signal-DFM: Roadnet-Guided Action-Token Flow Matching for Offline Traffic Signal Control**.

Signal-DFM is an offline traffic signal control framework for intelligent transportation systems. Instead of generating future traffic states and then recovering actions, Signal-DFM directly models the executable signal phase as a discrete action token. The learned discrete phase-flow score is combined with a roadnet-grounded PressLight / Max-Pressure-style pressure prior computed from CityFlow phase laneLinks.

> **Release status.** This repository is prepared as the public release entry point for the paper. The corresponding code, configuration files, and experiment scripts will be released in this repository upon paper acceptance.
