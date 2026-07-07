# AI Folder Usage

This folder contains an AI-generated iris classification workflow. Run everything from this directory.

## Files

| File | Purpose |
|---|---|
| `environment.yml` | Conda environment definition for running the notebook |
| `iris_classification.ipynb` | Loads iris data, trains classifiers, evaluates them, and selects the best model |

## Setup

Create and activate the conda environment:

```bash
cd assignment5/ai
conda env create -f environment.yml
conda activate assignment5-ai
```

If the environment already exists and you need to add updated packages:

```bash
conda env update -f environment.yml
```

## Run the Notebook

Launch Jupyter from this folder:

```bash
jupyter notebook iris_classification.ipynb
```

Run all cells in order. The notebook expects the iris dataset at `../data/iris.csv`.

## What the Notebook Does

1. Loads the iris CSV (no header row)
2. Splits the data into training and test sets
3. Trains several scikit-learn classifiers
4. Evaluates each model with 5-fold cross-validation and holdout test accuracy
5. Plots model accuracies and reports the best-performing classifier

## Requirements

The notebook uses Python 3.11 with `pandas`, `scikit-learn`, `matplotlib`, and `jupyter`, as listed in `environment.yml`.
