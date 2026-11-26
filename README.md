# Atlas Copilot

An enterprise support-and-knowledge copilot: ingests tickets and documents,
answers questions with citations, and will act through a team of agents.

## Setup
```bash
git clone https://github.com/<you>/atlas-copilot && cd atlas-copilot
uv sync            # creates .venv from uv.lock, dev tools included
```

## Run
```bash
uv run atlas --version
```

## Test and lint
```bash
uv run ruff check . && uv run ruff format --check .
uv run pytest
```

## Architecture
_Placeholder._ `src/atlas/` holds one package; modules arrive as the project grows:
`models/` (Day 2), `ingest/` (Day 3), `api/` (Day 4), `agents/` (later).