# rwth_rl_exercise_pixi_setup
A [Pixi](https://pixi.sh/) dev environment setup for my Reinforcement Learning course exercises at RWTH Aachen University.
This dev environment uses the [RLLBC](https://github.com/Data-Science-in-Mechanical-Engineering/RLLBC) Python library.

# Install Pixi
## Linux / MacOS
    curl -fsSL https://pixi.sh/install.sh | sh 

## Windows
    powershell -ExecutionPolicy ByPass -c "irm -useb https://pixi.sh/install.ps1 | iex"

# Clone the [RLLBC](https://github.com/Data-Science-in-Mechanical-Engineering/RLLBC) repository inside this repository folder
    git clone https://github.com/Data-Science-in-Mechanical-Engineering/RLLBC.git
    cd RLLBC

# Download the pixi.toml config file from this repo inside the RLLBC directory

# Install all dependencies
    pixi run uv pip sync ./RLLBC/requirements.txt 

# Start Jupyter Lab
    pixi run jupyter lab

..and voila! You've created a self-contained environment (using pixi) for Reinforcement Learning with all necessary dependencies!
