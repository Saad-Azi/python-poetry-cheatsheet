# Python Poetry Guide

## Setup & Usage

```bash
# Install Poetry
pip install poetry

# Initialize Poetry in your project
poetry init

# Install dependencies specified in pyproject.toml
poetry install

# Configure virtual environment to be within the project directory
poetry config virtualenvs.in-project true

# Activate virtual environment
poetry shell

# Deactivate virtual environment
exit

# View virtual environment information
poetry env info
poetry env info -p

# List all virtual environments
poetry env list

## Managing Packages
# Add a package
poetry add package_name

# Add a package with a specific version
poetry add package_name@version

# Add a package with minor updates
poetry add package_name^version

# Add a package with major updates
poetry add package_name~version

# Install dependencies without the project directory
poetry install --no-root

# View all installed packages
poetry show

# View details of a specific package
poetry show package_name

# Remove a package
poetry remove package_name

# Update all packages
poetry update

# Install the latest version of a package
poetry add package-name@latest

# Dependency Groups
# Define dependency groups in pyproject.toml
[tool.poetry.dependencies]
package_name = "^version"
python = "^3.9.0"

[tool.poetry.extras]
extras_name = ["package"]

# Add extras to a package
poetry add package_name --extras extras-name

# Add scripts in pyproject.toml
[tool.poetry.scripts]
script-name = "path.to.module:func"

# Run a script
poetry run script-name

## Updating Poetry
# Update Poetry to the latest minor version
poetry version minor
```

This file includes all the commands and configurations needed for working with Python Poetry, organized by category for clarity.
