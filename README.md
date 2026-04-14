# Setuptools with pyproject.toml and no setup.py

This is a companion example for the [setuptools](https://pydevtools.com/handbook/reference/setuptools/) reference page on the [Python Developer Tooling Handbook](https://pydevtools.com).

This package is an example project for building a Python package (i.e. wheel or sdist). It relies on [setuptools](https://setuptools.readthedocs.io/en/latest/) as a build backend with pyproject.toml for configuration.

## Commands:

> [!Note]
> setuptools does not manage your virtual environment. You will need to create and activate one yourself (e.g. with [venv](https://docs.python.org/3/library/venv.html)).

* Editable install:
```shell
# requires pip >= 21.3
python -m pip install -e .
```
* Run code:
```shell
python -c "import demo"
```
* Build:
```shell
python -m pip install build
python -m build
```
* Upload to PyPI:
```shell
python -m pip install twine
python -m twine upload dist/*
```