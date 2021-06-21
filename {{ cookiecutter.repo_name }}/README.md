# {{cookiecutter.project_name}}

{{cookiecutter.description}}


## Installation

Install conda environment and all python dependencies
```
make install
```


## Prepare Datasets

### Download raw data



### Make processed data from raw data
```
make data
```


## Usage

```
make <option>
```

Run `make help` for all available options
```
Available rules:

clean               Delete all compiled Python files 
data                Make Dataset 
download            Download Data from S3, no deletion 
install             Install mamba if not installed, then install conda environment with mamba 
lint                Lint using flake8 
pull                Download Data from S3, with deletion 
push                Upload Data to S3, with deletion 
upload              Upload Data to S3, no deletion 
```


## Project Organization
```
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── configs            <- Store all the hyper parameters in .yml files.
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in 
│
├── sandbox            <- Sandbox for anything that may not be included in other directories
│
├── environment.yml    <- The requirements file for reproducing the analysis environment.
│
├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io
```

---

Project based on the [cookiecutter data science project template](https://drivendata.github.io/cookiecutter-data-science/). #cookiecutterdatascience
