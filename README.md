# Assignment 5: Machine Learning with Iris

This assignment explores iris species classification using manual tutorials in Python and R, plus an AI-generated workflow in the `ai/` folder.

## Folder Structure

```
assignment5/
├── README.md              # This file
├── environment.yml        # Conda environment for manual notebooks (Python + R)
├── data/
│   └── iris.csv           # Iris dataset (150 rows, no header)
├── manual/
│   ├── ML_python.ipynb    # Step-by-step ML tutorial in Python
│   └── ML_R.ipynb         # Step-by-step ML tutorial in R
└── ai/
    ├── README_AI.md       # Usage guide for AI-generated files
    ├── PROMPTS.md         # Prompts used to generate the AI workflow
    ├── environment.yml    # Conda environment for the AI notebook
    └── iris_classification.ipynb
```



## Data

`data/iris.csv` contains 150 iris flower measurements with four numeric features and a species label:


| Column | Description                                                  |
| ------ | ------------------------------------------------------------ |
| 1      | Sepal length                                                 |
| 2      | Sepal width                                                  |
| 3      | Petal length                                                 |
| 4      | Petal width                                                  |
| 5      | Species (`Iris-setosa`, `Iris-versicolor`, `Iris-virginica`) |


The file has no header row.

## Manual Notebooks

The `manual/` folder contains tutorials adapted from Jason Brownlee's step-by-step machine learning guides ([Python](https://machinelearningmastery.com/machine-learning-in-python-step-by-step/) and [R](https://machinelearningmastery.com/machine-learning-in-r-step-by-step/))

- `manual/ML_python.ipynb` — Python workflow using scikit-learn
- `manual/ML_R.ipynb` — R workflow using caret



### Setup (manual)

Create and activate the assignment environment from the `assignment5` directory:

```bash
cd assignment5
conda env create -f environment.yml
conda activate assignment5
```

Launch JupyterLab:

```bash
jupyter lab
```

Open the notebook you want from the `manual/` folder. Update any hard-coded data paths in the Python notebook to point to `data/iris.csv` if needed.

The manual environment includes Python packages (`pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `jupyterlab`) and R packages (`caret`, `ggplot2`, `randomforest`, etc.) with the IR kernel for R notebooks.

## AI-Generated Workflow

The `ai/` folder contains a separate AI-generated iris classification notebook with its own conda environment. See `ai/README_AI.md` for setup and usage instructions.

## Quick Start

**Manual Python tutorial:**

```bash
cd assignment5
conda env create -f environment.yml
conda activate assignment5
jupyter lab manual/ML_python.ipynb
```

**AI-generated notebook:**

```bash
cd assignment5/ai
conda env create -f environment.yml
conda activate assignment5-ai
jupyter notebook iris_classification.ipynb
```

Both workflows use the shared dataset at `data/iris.csv`.