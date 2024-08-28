# Deep Reinforcement Learning for Power Distribution System Reconfiguration

This repository implements three deep reinforcement learning (RL) algorithms: PPO, A2C, and TRPO, to reconfigure power distribution systems and maximize load supply during disasters.

## Overview

- **Environment:** 
  - The IEEE 34 test system is used as the environment for the RL algorithms.
  - The environment is sourced from [this repository](https://github.com/Jubeyer/RL-to-Reconfigure-Microgrid) with a few modifications.
  
- **Modifications:** 
  - Added a Convolutional Neural Network (CNN) as a feature extractor.
  - Conducted comprehensive simulation cases in both normal and post-disaster conditions.
  - Tested A2C and TRPO algorithms alongside PPO.

## Instructions for Running the Code

- **Notebooks:** 
  - Two Jupyter notebooks are provided for running the simulations:
    - `run_normal.ipynb`: Reconfigure the system during normal conditions.
    - `run_post_fault.ipynb`: Reconfigure the system during post-disaster conditions.

- **Environment Setup:**
  - The following files are related to the RL environment settings:
    - `DGs.py`, `DSS_CircuitSetup.py`, `DSS_Initialize.py`, `ieee34Mod1.dss`, `IEEELineCodes.dss`, `openDSSenv34.py`, `state_action_reward.py`, `switch.py`.

## Additional Requirements

- **TensorBoard:** 
  - Required to view the figures generated after the simulation.

- **Operating System:**
  - As the OpenDSS software is supported on Windows, this repository requires a Windows PC to run.

- **Python Version:**
  - The code is tested with Python 3.8.10.

- **Dependencies:**
  - Install the required Python libraries from the `requirements.txt` file.
  
  ```bash
  pip install -r requirements.txt
