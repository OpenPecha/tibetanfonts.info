
# Coding guidelines
## General

- Use [OpenPecha Project Template](https://github.com/OpenPecha/openpecha-project-template/generate) to create new project.
- `python` version should be >= `3.8`.
- Every project should be a Python installable `python package`.
  - [Packaging Python projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
  - [Packages and importing modules](https://docs.python.org/3/tutorial/modules.html#packages)
- `pre-commit` to ensure all code changes follow OpenPecha's code quality standards.

### Coding style

- [`Black`](https://github.com/psf/black) (code formatter)
- [`flake8`](https://github.com/PyCQA/flake8) (linter)
- [`mypy`](https://github.com/python/mypy) (static type checker)

### Documentation

- [pydocsstyle](https://github.com/PyCQA/pydocstyle)
- [Google Style Python Docstring](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)

### Testing

- [`pytest`](https://github.com/pytest-dev/pytest) (unit test)
- [`coverage.py`](https://github.com/nedbat/coveragepy) (test coverage should be above 80%)

---

## Project setup

### Prerequisites

- Make sure you have created your project repo using the [OpenPecha project template](https://github.com/OpenPecha/openpecha-project-template/generate).
- Make sure you have cloned your repo onto your local machine.
- Make sure you are inside your project repo.

### 1. Environment setup

1.1. Create environment

```bash
python3 -m venv .venv
```

1.2. Activate environment

1.2.1 Mac/Linux

```bash
source .venv/bin/activate
```

1.2.2 Window

```cdm
 .\venv\Scripts\activate
```

### 2. Installation

```bash
pip install -U pip
pip install -e .
pip install .[dev]
pre-commit install
```

> Note: `zsh` users need to escape `[]`, like `\[dev\]`

---

## Development

### Add dependencies

```python
[project]
...
dependencies = [
  "openpecha>=0.8.21",
  "antx>=0.1.4",
]
```

---

## Testing

```bash
PYTHONPATH=src pytest
PYTHONPATH=src pytest --cov <project_name>
```
> **Note**: Please, replace `<project_name>` with your project name.

### Test coverage details
```bash
coverage html
```

Then open `./htmlcov/index.html` in your preferred web browser.

---
### Need help?
- Contact [Tenzin](https://github.com/10zinten) or [Tenzin Kaldan](https://github.com/kaldan007) on [Discord](https://discord.com/invite/7GFpPFSTeA). 
