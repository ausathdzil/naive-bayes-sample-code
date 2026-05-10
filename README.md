# Local Development

This repository contains Jupyter notebooks and a small Python setup managed by `pyproject.toml`.

## Prerequisites

- Python 3.14 or newer
- `uv` installed

Install `uv` (one-time):

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

macOS (Homebrew):

```bash
brew install uv
```

Windows (PowerShell):

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

## Setup

From the repository root:

```bash
uv venv .venv
source .venv/bin/activate
uv pip install -e .
```

Alternatively, use `uv sync`:

```bash
uv sync
source .venv/bin/activate
```

## Run Notebooks

```bash
uv run jupyter notebook
```

Open one of the notebooks under `notebooks/` (for example, `mushroom.ipynb`).

## Dependencies

Core dependencies are defined in `pyproject.toml` and include:

- `notebook`
- `pandas`
- `scikit-learn`
