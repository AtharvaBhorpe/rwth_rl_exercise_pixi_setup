# rwth_rl_exercise_pixi_setup
A [Pixi](https://pixi.sh/) dev environment setup for my Reinforcement Learning course exercises at RWTH Aachen University.
This dev environment uses the [RLLBC](https://github.com/Data-Science-in-Mechanical-Engineering/RLLBC) Python library.

# 1. Install Pixi
## Linux / MacOS
    curl -fsSL https://pixi.sh/install.sh | sh 

## Windows
    powershell -ExecutionPolicy ByPass -c "irm -useb https://pixi.sh/install.ps1 | iex"

# 2. Clone the [RLLBC](https://github.com/Data-Science-in-Mechanical-Engineering/RLLBC) repository inside this repository folder
    git clone https://github.com/Data-Science-in-Mechanical-Engineering/RLLBC.git
    cd RLLBC

# 3. Download the [pixi.toml](https://github.com/AtharvaBhorpe/rwth_rl_exercise_pixi_setup/blob/main/pixi.toml) config file from this repo inside the RLLBC directory

# 4. Install all dependencies
    pixi run uv pip sync ./requirements.txt 

# 5. Start Jupyter Lab
    pixi run jupyter lab

..and voila! You've created a self-contained environment (using pixi) for Reinforcement Learning with all necessary dependencies!
