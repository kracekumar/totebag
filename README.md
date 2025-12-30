# Totebag

A Terminal User Interface (TUI) for managing `uv` Python projects.

## Overview

Totebag provides an intuitive, interactive CLI tool for Python developers to manage their projects using `uv` - a fast Python package installer and resolver. Instead of remembering and typing complex `uv` commands, developers can navigate through a rich terminal interface to perform common project management tasks.

## Tech Stack

- **Framework**: [Textual](https://textual.textualize.io/) - Python TUI framework
- **Package Manager**: [uv](https://github.com/astral-sh/uv) - Fast Python package installer
- **Autocomplete**: [textual-autocomplete](https://github.com/darrenburns/textual-autocomplete) - Autocomplete widgets for Textual
- **Code Quality**: [Ruff](https://github.com/astral-sh/ruff) - Fast Python linter and formatter
- **Testing**: [pytest](https://pytest.org/) - Testing framework

## Requirements

- Python 3.11+
- uv (installed independently)

## Installation

```bash
# Clone the repository
git clone https://github.com/kracekumar/totebag.git
cd totebag

# Install with uv
uv sync
```

## Development

### Setup

```bash
# Sync dependencies
uv sync

# Install dev dependencies
uv pip install -e ".[dev]"
```

### Testing

```bash
# Run all tests
uv run pytest

# Run with coverage
uv run pytest --cov=src

# Run specific test file
uv run pytest tests/test_models.py
```

### Code Quality

```bash
# Run linter
uv run ruff check .

# Format code
uv run ruff format .

# Check formatting
uv run ruff format --check .
```

## Usage

```bash
# Run totebag
totebag
```

## Project Status

🚧 **Early Development** - Initial project setup phase

## License

MIT

## Author

kracekumar
