# memolane

Learning project: clean Flask API with tests

## What it does

- pytest coverage for the happy paths
- SQLite storage via sqlite3 stdlib
- Request validation and consistent error shape
- CRUD endpoints for notes

## Install

```bash
pip install -r requirements.txt
flask --app app run --debug
```

## Examples

```bash
curl -X POST localhost:5000/notes \
  -H 'content-type: application/json' \
  -d '{"title": "first", "body": "hello"}'
```

## Project structure

```text
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_api.py
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── app.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
