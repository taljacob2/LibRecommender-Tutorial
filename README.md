# LibRecommender Tutorial

## Setup

1. [Install conda](https://conda.io/projects/conda/en/latest/user-guide/install/rpm-debian.html)

   - Add `source` Shortcut:

     To add the `conda` command to the bash terminal, use its shortcut reference in the terminal, by adding the following `source` line to a .bashrc file:

     ```sh
     source /opt/conda/etc/profile.d/conda.sh
     ```

     - To add for the entire System (which includes all Users), add it to `etc/bash.bashrc`
     - To add for the current User, add it to `~/.bashrc`

1. Create a virtual environment

   ```
   conda create -n new_env python=3.11
   conda activate new_env
   ```

1. Install packages from `requirements.txt`:

   ```
   pip install -r requirements.txt
   ```

## Development

1. Install packages from `requirements-dev.txt`:

   ```
   pip install requirements-dev.txt
   ```

1. Run jupyter notebook:

   ```
   jupyter notebook --NotebookApp.token=''
   ```

   The jupyter notebook app will serve at: http://localhost:8888/lab

1. Go to http://localhost:8888/lab

   - To run python script inside jupyter notebook:

     Open a "Console", and use `%run <name-of-script.py>` as an entry in a cell, and execute it.

## Docs

See [LibRecommender Docs](/docs/LibRecommender.md)
