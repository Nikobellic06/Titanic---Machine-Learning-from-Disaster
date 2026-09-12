# Titanic: Machine Learning from Disaster

This project is a machine learning solution for the classic Kaggle Titanic survival prediction challenge. The goal is to predict whether a passenger survived based on features such as age, sex, ticket class, fare, family size, and embarkation details.

## Project overview

The repository contains an exploratory data analysis workflow and model experimentation focused on understanding which factors influence survival and selecting a strong predictive pipeline.

## Folder structure

- `Dataset/` – contains the training and test datasets, plus the expected submission format
- `notebbook/` – Jupyter notebook with the exploratory analysis and preprocessing steps
- `graphs/` – output plots and visualizations generated during analysis
- `pipelines/` – intended location for reusable model/prediction pipelines
- `submissions/` – CSV files with candidate submission outputs

## Dataset

The Titanic dataset is typically provided by Kaggle and includes:

- `train.csv` – labeled training data with the `Survived` target column
- `test.csv` – unlabeled test data used for prediction
- `gender_submission.csv` – sample submission format for Kaggle

Key features explored in the analysis include:

- `PassengerId`
- `Pclass` (ticket class)
- `Name`
- `Sex`
- `Age`
- `SibSp`
- `Parch`
- `Ticket`
- `Fare`
- `Cabin`
- `Embarked`

## Workflow

The notebook in `notebbook/TitanicEDA.ipynb` covers:

1. Loading the dataset
2. Handling missing values
3. Feature engineering
4. Exploratory data analysis and visualizations
5. Preprocessing for machine learning models
6. Model comparison and tuning
7. Generating predictions for submission

## Dependencies

This project uses Python libraries commonly used in data science and ML, including:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- Jupyter Notebook

You can install the main dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## How to run

Open the notebook:

```bash
jupyter notebook notebbook/TitanicEDA.ipynb
```

Or run the notebook in VS Code with the Jupyter extension enabled.

## Notes

- The project is intended for learning and experimentation in a Kaggle-style ML workflow.
- Submission files in `submissions/` represent iterative model outputs and can be compared for performance.
- The dataset is not tracked as a git repository artifact here, so it should be downloaded or provided separately if needed.

## Goal

The objective is to build a model that predicts whether a passenger survived the Titanic disaster with the best possible accuracy.
