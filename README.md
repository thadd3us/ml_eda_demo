# Machine Learning (ML) and Exploratory Data Analysis (EDA) Demo

* This repository is for a hands-on ML presentation in October 2023 for the Tropini Lab.
* Please go through the setup steps to get a working conda environment on your machine prior to the presentation.

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
git clone git clone https://github.com/thadd3us/ml_eda_demo.git
```

#### Create the conda/micromamba environment

```bash
cd ml_eda_demo
micromamba remove --name ml_eda_demo --all  # Optional cleanup if you already created the environment once.
micromamba env create -f environment.yml
```

### Windows setup

I'm not really sure, I haven't used Windows in ages :)

If you use Windows and have trouble adapting the Mac steps above, please let me know, I might be able to help.  Feel free to use `conda` instead of `micromamba`, especially if you have it already.

---
# SETUP ENDS HERE
---

## Running things in the environment

### Activate the environment (once per terminal session)

```bash
cd ml_eda_demo
micromamba activate ml_eda_demo
```

### Starting a jupter notebook in the environment

```bash
jupyter notebook \
    --NotebookApp.allow_origin='https://colab.research.google.com' \
    --port=8888 \
    --NotebookApp.port_retries=0
```

