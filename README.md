# Finan

Train language models from scratch in PyTorch.

`notebook.ipynb` is the lab. `src/finan/` is an empty package to fill as cells settle.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
```

Then open `notebook.ipynb` and keep working cell by cell.

## Layout

```
notebook.ipynb     lab
src/finan/         package skeleton
data/              downloaded training text
checkpoints/       saved weights
tests/             package smoke tests
```

## Current stage

Tokenization (GPT-2 BPE), a sliding-window next-token dataset, and token + positional embeddings.

Next: attention → GPT block → pretraining → generation.
