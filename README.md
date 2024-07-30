# FastAPI Backend

This project is a FastAPI backend application designed to provide a RESTful API. It uses Poetry for dependency management.

## Prerequisites

Ensure you have Poetry installed. You can install it by following the instructions here: [Install Poetry](https://python-poetry.org/docs/).
THEN *** poetry config virtualenvs.in-project true


## Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/fastapi-backend.git
   cd fastapi-backend

2. **Install Poetry (wsl):**
   ```bash
   sudo apt update && sudo apt upgrade -y

   # remove Python3.10
   sudo apt-get purge --auto-remove python3 -y

   # install python3.12
   sudo apt-get install software-properties-common -y
   sudo add-apt-repository ppa:deadsnakes/ppa -y
   sudo apt update
   sudo apt install python3.12 -y

   # version check python3
   python3 --version    #3.12 나오면 정상

   # install poetry (pipx)
   sudo apt install pipx -y
   pipx install poetry

   # env setting
   sudo vi ~/.bashrc
   # add last line
   PATH="$HOME/.local/bin:$PATH"
   # run source command
   source ~/.bashrc

   # 
   cd LTGT-backend
   poetry config virtualenvs.in-project true
   poetry install
   poetry shell
