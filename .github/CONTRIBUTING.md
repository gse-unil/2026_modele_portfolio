# Contributing to 2026_Geoinformatique_II

## Setup (local)

This project is built with [Jupyter Book](https://jupyterbook.org/stable).

### 1. Install dependencies

More info [here](https://jupyterbook.org/stable/get-started/install/).

```bash
# create env ...
mamba install -c conda-forge "jupyter-book"
# or
# pip install "jupyter-book>=2.0.0"
```

### 2. Clone the repository

```bash
git clone https://github.com/gse-unil/2026_Geoinformatique_II.git
cd 2026_Geoinformatique_II
```

### 4. Run locally

```bash
jupyter-book start
```

## Adding Content

* Use Markdown (.md) or Jupyter notebooks (.ipynb)
* Add content to the relevant section
* Include exercises when appropriate
* For the table of contents:
  * Add new files to the `myst.yml` toc section
