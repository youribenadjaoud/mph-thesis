# MPH Thesis Project
This repository holds all necessary code for Youri Benadjaoud's MPH Thesis at Brown University School of Public Health

## Requirements

To run the code in this repository, you will need Python 3.7.1+ and R 4.0.2+ pre-installed.

In Python, we use [`poetry`](https://python-poetry.org/) to manage our dependencies. In R, we use [`renv`](https://rstudio.github.io/renv/articles/renv.html).
To install these dependency managers, you can run (assumes Mac or Linux; see tools' documentation for other operating systems):

```bash
curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python3 -
Rscript -e 'if(!requireNamespace("remotes")){install.packages("remotes");remotes::install_github("rstudio/renv")} else {remotes::install_github("rstudio/renv")}'
```

Once these are installed, you can install all dependencies with

```bash
poetry install
Rscript -e 'renv::restore()'
```
