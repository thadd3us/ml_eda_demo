# Machine Learning and Exploratory Data Analysis Demo

## Setup

You will need a working conda installation.

I recommend micromamba, a faster conda implementation.

See: 
* https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html
* https://mamba.readthedocs.io/en/latest/micromamba-installation.html#umamba-install

### Macos

#### Get homebrew (if you don't have it)
See: https://brew.sh/
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```sh
brew install micromamba
# Then run the command it tells you to add micromamba to your shell.
```

### Clone the repo

```sh
git clone ???
cd
```

### Create the environment (once per machine)

```sh
# Optional cleanup if you already did this.
micromamba remove --name ml_eda_demo --all
micromamba env create -f environment.yml
```

### Activate the environment (once per terminal session)

```sh
conda activate ml_eda_demo
```

