# PF_LQR — Pick and Throw Robot Dynamics

Overview
- Purpose: Implementations and experiments for the PF-LQR controller used with the pick-and-throw robot. This folder contains code, configs, and examples to develop and evaluate the LQR-based control strategy for trajectory tracking, path-following, and stability during throw maneuvers.
- Note: PF-LQR here refers to the LQR-based controller variant used in this project — replace the expansion if you prefer a different meaning (e.g., Path-Following LQR, Proportional-Feedback LQR).

Repository context
- Repo: Jash-2000/Pick_and_Throw_Robot_Dynamics — "Exploring Advance Topics of Control Systems".
- This folder focuses on: LQR controller design, simulation experiments, and analysis scripts related to pick-and-throw maneuvers.

Folder structure
- src/ — source code for the PF-LQR controller and supporting utilities (Python or MATLAB).
- models/ — robot models used by controllers (URDF, Simulink .slx, or .mat files).
- configs/ — configuration files (YAML/JSON) for experiments and controller parameters.
- notebooks/ — analysis and visualization notebooks (Jupyter or MATLAB Live Scripts).
- data/ — saved simulation logs and result files.
- examples/ — runnable examples, demo scripts, and launch sequences.

Prerequisites
- Python 3.8+ (if Python is used)
  - Recommended packages: numpy, scipy, control, matplotlib, pyyaml
  - Install with: pip install -r requirements.txt (if provided)
- MATLAB/Simulink (optional) if .slx or MATLAB scripts are included

Installation
1. Clone the repository:
   git clone https://github.com/Jash-2000/Pick_and_Throw_Robot_Dynamics.git
2. Change to the PF_LQR folder and install dependencies (if applicable):
   cd PF_LQR
   pip install -r requirements.txt

Running simulations / examples
- To run a Python-based example (replace with actual entrypoint if different):
  python src/run_pf_lqr.py --config configs/pf_lqr_config.yaml

- To open and run MATLAB/Simulink models:
  Open models/pick_and_throw_pf_lqr.slx in MATLAB/Simulink and run any demo scripts in scripts/ (if present).

Configuration
- Controller and experiment parameters are stored in configs/*.yaml or configs/*.json. Edit these to change LQR weights, discretization, initial conditions, and simulation parameters.

Files of note (update names if different)
- src/run_pf_lqr.py — main entry to launch PF-LQR simulations and experiments.
- src/pf_lqr_controller.py or src/pf_lqr.m — LQR formulation and controller interface.
- src/dynamics.py or src/dynamics.m — robot dynamics used by the controller.
- configs/pf_lqr_config.yaml — default configuration used by examples.
- models/pick_and_throw_model.urdf or .slx — robot model files used for simulation.
- notebooks/analysis.ipynb — notebooks to reproduce plots and analyze results.

Outputs & results
- Simulation outputs are saved to data/ by default. Filenames and output formats can be configured in configs/*.yaml.
- Use notebooks/plot_results.ipynb to reproduce figures and performance metrics used in reports.

Contributing
- Open an issue for feature requests or bug reports.
- Fork the repository, create a feature branch, and submit a pull request. Include clear descriptions and reproduction steps for experiments.

License
- Specify the license for this folder/project in the repository root (e.g., MIT). If desired, add a LICENSE file to the repo root.

Contact
- Maintained by Jash-2000. For help, open an issue in this repository.

Notes
- Replace placeholder filenames above with the actual script/model names present in this folder. If you want, I can inspect the repository and update the README to reference exact files and commands.