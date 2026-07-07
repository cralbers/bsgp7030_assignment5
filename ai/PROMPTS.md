# Prompts Used to Generate Files in `ai/`

The files in this folder were created using the following prompts, in order.

## 1. Initial notebook request

> Working in the assignment5/ai directory and given the data/iris.csv, build a notebook that loads it, splits the data into train and test sets, trains a few classifiers, evaluates them, and picks the best based on accuracy. Do not look at any files in any directory other than the data/iris.csv data file.

**Generated:** `iris_classification.ipynb` (initial version)

## 2. Add cross-validation

> Instead of evaluating the models based on only accuracy_score, run k-fold cross-validation as well.

**Updated:** `iris_classification.ipynb`

## 3. Add environment file

> Additionally create an environment.yml file that allows for recreation of the environment and packages necessary to run the notebook

**Generated:** `environment.yml`

## 4. Implement the plan

> Implement the plan as specified, it is attached for your reference. Do NOT edit the plan file itself.

**Generated/updated:** `iris_classification.ipynb`, `environment.yml`

## 5. Add accuracy graph

> add a graph to the @assignment5/ai/iris_classification.ipynb notebook that graphs the accuracy of each pf the evaluated models

**Updated:** `iris_classification.ipynb`, `environment.yml` (added `matplotlib`)

## 6. Add code annotations

> add code annotations to @assignment5/ai/iris_classification.ipynb to explain the code

**Updated:** `iris_classification.ipynb`

## 7. Add README

> create a readme file in the ai folder called README_AI.md that only explains the usage of the files in the ai folder

**Generated:** `README_AI.md`

## 8. Add this prompts file

> generate a file called PROMPTS.md int e ai folder that lists the prompts used to generate the files in the folder

**Generated:** `PROMPTS.md`
