# 3d-models

Personal CadQuery projects and experiments.

## Development Setup

This repo is currently using the full `uv` route. The CadQuery stack installed
successfully in WSL with a repo-local `.venv`.

Install `uv` in WSL if needed:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Install or refresh the project environment:

```bash
uv sync
```

Run the smoke test:

```bash
uv run scripts/smoke_test.py
```

Open the repo in VS Code from WSL:

```bash
code .
```

In VS Code, select the interpreter at `.venv/bin/python`. For model viewing,
install the VS Code extensions `Python`, `Remote - WSL`, and `OCP CAD Viewer`.

## Current Workflow

1. Create each model under `parts/<model_name>/`.
2. Keep the source model in `model.py`.
3. Export generated files to that part's `exports/` directory.
4. Store screenshots or rendered previews in that part's `images/` directory.
5. Link each part from this README as the repo grows.
