# Machine Learning (ML) and Exploratory Data Analysis (EDA) Demo

* This repository is for a hands-on ML presentation in October 2023 for the Tropini Lab.
* Please 

## Setup

### Macos setup

Suggested setup:

#### Get [homebrew](https://brew.sh/)

See: https://brew.sh/
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### Get git and micromamba

```bash
brew install git micromamba
# Then run the command it tells you to add micromamba to your shell.
```

Micromamba is a faster conda implementation.  See: 
* https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html
* https://mamba.readthedocs.io/en/latest/micromamba-installation.html#umamba-install


#### Clone the repo

```bash
git clone ???
cd
```

### Create the environment (once per machine)

```bash
micromamba remove --name ml_eda_demo --all  # Optional cleanup if you already did this.
micromamba env create -f environment.yml
```

### Windows setup

I'm not really sure.

If you use Windows and have trouble adapting the Mac steps above, please let me know.


## Running things in the environment

### Activate the environment (once per terminal session)

```bash
conda activate ml_eda_demo
```

```bash
jupyter notebook \
    --NotebookApp.allow_origin='https://colab.research.google.com' \
    --port=8888 \
    --no-browser \
    --NotebookApp.port_retries=0
```

