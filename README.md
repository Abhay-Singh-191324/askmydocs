# askmydocs

Tiny retrieval pipeline: TF-IDF chunks + pluggable LLM step

Side project, maintained when I have time.

## Usage

```bash
python rag.py ./notes "how do I rotate logs?"
```

## Installation

```bash
pip install -r requirements.txt
```

## Highlights

- Swap in any LLM for the answer step
- TF-IDF retrieval: zero external services needed
- Chunk markdown with overlap, keep source paths
- Prints sources with scores for transparency

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── data/
│   └── sample.md
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── rag.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
