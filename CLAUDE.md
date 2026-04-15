# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Spendly — a Flask-based expense tracking web application. Educational project where students implement features step-by-step (auth, CRUD, filtering).

## Commands

```bash
# Run the application
python app.py

# Run tests
pytest

# Run a single test file
pytest tests/test_<file>.py

# Run a specific test
pytest tests/test_<file>.py::test_<name>
```

## Architecture

- **app.py** — Flask application entry point; defines routes and renders templates
- **templates/** — Jinja2 HTML templates (base.html + page templates)
- **static/** — CSS (`css/style.css`) and JavaScript (`js/main.js`)
- **database/** — SQLite database layer (`db.py`)

## Implementation Status

| Component | Status |
|-----------|--------|
| Landing page | Complete |
| Auth routes (`/login`, `/register`, `/logout`) | Partial — routes exist, no logic |
| Profile page | Placeholder |
| Expense CRUD (`/expenses/add`, `/expenses/:id/edit`, `/expenses/:id/delete`) | Placeholder |
| Database layer (`get_db`, `init_db`, `seed_db`) | To be implemented |

## Dependencies

- Flask 3.1.3
- Werkzeug 3.1.6
- pytest 8.3.5
- pytest-flask 1.3.0
