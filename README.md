## Data Science Project Template

This template is mainly inspired by the [Cookiecutter Data Science project structure](https://drivendata.github.io/cookiecutter-data-science/) that aims to be a logical, reasonably standardized, but flexible project structure for doing and sharing data science work.

We also recommends to track, manage and share models with MLFlow and Neptune (https://github.com/neptune-ai/neptune-mlflow).

### Folder structure
- `data`: Datasets.
- `docs`: Sphinx documentation. 
- `models`: Trained and serialized models, model predictions, or model summaries.
- `notebooks`: Jupyter notebooks. Naming convention is the date (for ordering), the creator's initials, and a short `-` delimited description, e.g. `1.0-jqp-initial-data-exploration`.
- `references`: Data dictionaries, manuals, and all other explanatory materials.
- `reports`: Generated analysis as HTML, PDF, LaTeX, etc.
- `src`: Stores source code (python, R etc) which serves multiple scenarios. During data exploration and model training, we have to transform data for particular purpose. We have to use same code to transfer data during online prediction as well. So it better separates code from notebook such that it serves different purpose.


```
.
├── .env               <- Store your secrets and config variables in a special file
├── .gitignore         <- Avoids uploading data, credentials, 
|                         outputs, system files etc
├── env                <- Will contain the Python executable files and installed libraries for your virtualenv environment
├── requirements.txt   <- Install the environment dependencies with: `pip install -r requirements.txt`
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
├── docs               <- Space for Sphinx documentation
├── models             <- Trained and serialized models, model predictions, or model summaries
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│   |                     the creator's initials, and a short `-` delimited description, e.g.
│   |                     `1.0-jqp-initial-data-exploration`.
│   ├── eda            <- Placholder for describing exploratory data analysis
│   ├── evaluation     <- Placholder for describing model evaluation
│   ├── modeling       <- Placholder for describing how the model is built
│   └── poc            <- Describing Proof-of-Concept
├── references         <- Data dictionaries, manuals, etc.
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   ├── build_features.py
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
└── tox.ini               <- Automate testing, cf. https://tox.readthedocs.io/en/latest/.
```

### References
* [Complete Data Science Project Template with Mlflow for Non-Dummies](https://towardsdatascience.com/complete-data-science-project-template-with-mlflow-for-non-dummies-d082165559eb)
* [MLflow Documentation](https://www.mlflow.org/docs/latest/index.html)
* [Manage your Data Science project structure in early stage](https://towardsdatascience.com/manage-your-data-science-project-structure-in-early-stage-95f91d4d0600)
* [GitHub repo of an example data science project using Mlflow](https://gitlab.com/jan-teichmann/ml-flow-ds-project)
* [A logical, reasonably standardized, but flexible project structure for doing and sharing data science work](https://drivendata.github.io/cookiecutter-data-science/#data-is-immutable) & [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science/)
* [How to Structure a Python-Based Data Science Project](https://medium.com/swlh/how-to-structure-a-python-based-data-science-project-a-short-tutorial-for-beginners-7e00bff14f56)
