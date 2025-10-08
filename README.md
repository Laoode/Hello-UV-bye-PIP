# UV Package Manager

UV is 100x faster than pip because it's written in Rust.

## Installation

Install UV using pip:

```bash
pip install uv
```

## Verify Installation

Check if UV has been installed:

```bash
uv
```

## Python Version Management

### List Available Python Versions

Check available Python versions:

```bash
uv python list
```

### Install Specific Python Version

Install a particular Python version:

```bash
uv python install 3.12
```

### Find Python Version

Search for a particular version:

```bash
uv python find 3.12
```

### Uninstall Python Version

Uninstall a Python version:

```bash
uv python uninstall 3.12
```

## Running Python Scripts

### Basic Run

Run a Python script:

```bash
uv run main.py
```

### Run with Specific Python Version

Specify a Python version when running a script:

```bash
uv run --python 3.9.21 main.py
```

### Run with Dependencies

Run a Python script with dependencies that haven't been installed yet:

```bash
# Script uses rich and requests
uv run --with rich --with requests --python 3.9.12 main.py
```

## Project Management

### Create New Project

Initialize a new project with UV:

```bash
uv init
```

### Add Dependency

Add a dependency to your project:

```bash
uv add requests
```

### Remove Dependency

Remove a dependency from your project:

```bash
uv remove requests
```

### Create venv

Create a virtual environment with uv:

```bash
uv venv
# . .venv\Scripts\activate
```

### Install and Synchronize the Package

This will install the package from `pyproject.toml`:

```bash
uv sync
```


