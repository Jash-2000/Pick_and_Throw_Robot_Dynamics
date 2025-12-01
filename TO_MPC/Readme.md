# TO_MPC — Pick and Throw Robot Dynamics

Overview
- Purpose: Implementations and experiments for Time-Optimal Model Predictive Control (TO-MPC) applied to the pick-and-throw robot. This folder contains code, configs, and examples used to develop and evaluate MPC-based controllers for trajectory planning and throw maneuvers.

Repository context
- Repo: Jash-2000/Pick_and_Throw_Robot_Dynamics — "Exploring Advance Topics of Control Systems".
- This folder focuses on: Time-Optimal MPC design, simulation setups, and scripts to reproduce related experiments.

Folder structure
- src/ — source code for the TO-MPC controllers and utilities (Python/MATLAB as applicable).
- models/ — robot models used by the controllers (URDF, Simulink .slx, or .mat files).
- configs/ — configuration files (YAML/JSON) for experiments and controller parameters.
- notebooks/ — analysis and visualization notebooks (Jupyter or MATLAB Live Scripts).
- data/ — saved simulation logs and result files.
- examples/ — runnable examples and launch scripts.

Prerequisites
- Python 3.8+ (if Python is used)
  - Recommended packages: numpy, scipy, casadi (or other optimizer), matplotlib, pyyaml
  - Install with: pip install -r requirements.txt (if a requirements.txt is provided)
- MATLAB/Simulink (optional) if .slx or MATLAB scripts are included
- Optimization solvers: IPOPT, OSQP, or the solver specified in configs/

Installation
1. Clone the repository:
   git clone https://github.com/Jash-2000/Pick_and_Throw_Robot_Dynamics.git
2. Change to the TO_MPC folder and install Python dependencies (if applicable):
   cd TO_MPC
   pip install -r requirements.txt

Running simulations / examples
- To run a Python-based example (replace with actual entrypoint if different):
  python src/run_mpc.py --config configs/mpc_config.yaml

- To open and run MATLAB/Simulink models:
  Open models/pick_and_throw_mpc.slx in MATLAB/Simulink and run the demo script in scripts/ (if present).

Configuration
- Controller and experiment parameters are stored in configs/*.yaml or configs/*.json. Edit these files to change controller horizons, weights, solver options, and initial conditions.

Files of note (update names if your code differs)
- src/run_mpc.py — main entry point to launch TO-MPC simulations and experiments.
- src/mpc_controller.py — MPC formulation and solver interface.
- src/dynamics.py — robot dynamics used by the MPC (discrete/continuous-time).
- configs/mpc_config.yaml — default MPC configuration used by examples.
- models/pick_and_throw_model.urdf or .slx — robot model files used for simulation.
- notebooks/analysis.ipynb — scripts and notebooks to reproduce plots and analyze results.

Outputs & results
- Simulation outputs are saved to data/ by default. Filenames and output formats can be configured in configs/*.yaml.
- Use notebooks/plot_results.ipynb to reproduce figures and performance metrics for experiments.

Contributing
- Open an issue for feature requests or bug reports.
- Fork the repository, create a feature branch, and submit a pull request. Include clear descriptions and any reproduction steps.

License
- Specify the license for this folder/project in the repository root (e.g., MIT). If you want, add a LICENSE file to the repo root.

Contact
- Maintained by Jash-2000. For help, open an issue in this repository.

Notes
- Replace placeholder filenames above with the actual script/model names present in this folder. If you want, I can inspect the repository and update the README to reference exact files and commands.