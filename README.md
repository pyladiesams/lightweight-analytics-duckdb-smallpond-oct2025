# Lightweight Analytics at Scale: Hands-On with DuckDB & Smallpond in Python
### Presentation: [{ Lightweight Analytics at Scale }](https://github.com/pyladiesams/lightweight-analytics-duckdb-smallpond-oct2025/blob/main/workshop/Smallpond%20Pyladies%20Amsterdam.pdf)

## Workshop description
In this workshop, you’ll learn how to build powerful yet lightweight data workflows using Python, DuckDB, and Smallpond. We’ll explore how DuckDB enables fast, in-process SQL analytics on massive datasets without heavy infrastructure, and how Smallpond extends those capabilities into distributed, collaborative, or cloud-friendly environments.

## Requirements
* PyLadies Amsterdam uses [uv](https://docs.astral.sh/uv/) for dependency management
* Google account if you want to use [Google Colab](https://colab.research.google.com/)
* [Docker desktop](https://docs.docker.com/desktop/) or Docker + Docker compose 
 
## Usage
### with uv
Run the following code:
```bash
git clone https://github.com/pyladiesams/lightweight-analytics-duckdb-smallpond-oct2025.git
cd lightweight-analytics-duckdb-smallpond-oct2025

# create and activate venv, install dependencies
uv sync
```
### with Google Colab
1. Visit [Google Colab](https://colab.research.google.com/)
2. In the top left corner select "File" &#8594; "Open Notebook"
3. Under "GitHub", enter the URL of the repo of this workshop
4. Select one of the notebooks within the repo.
5. At the top of the notebook, add a Code cell and run the following code:
```bash
!git clone https://github.com/pyladiesams/lightweight-analytics-duckdb-smallpond-oct2025.git
%cd lightweight-analytics-duckdb-smallpond-oct2025
!pip install -r requirements.txt
```
### for a workshop giver
To get started, open the `pyproject.toml` file and set the required Python version. The pre-selected version 3.8 is generally a safe choice for most use cases.

After you have specified the Python version, you can create a virtual environment with `uv venv` and add packages with `uv add <package>`. Before the workshop, you can generate a requirements.txt file, which is needed e.g. for running code in Google Colab, by running `uv export > requirements.txt`.

## Video record
Re-watch [this YouTube stream](https://www.youtube.com/live/rBDs6izPsLE)

## Credits
This workshop was set up by @pyladiesams and @valerybriz

## Appendix
### Pre-Commit Hooks

To ensure our code looks beautiful, PyLadies uses pre-commit hooks. You can enable them by running `pre-commit install`. You may have to install `pre-commit` first, using `uv sync`, `uv pip install pre-commit` or `pip install pre-commit`.

Happy Coding :)
