# poetry-cheatsheet
Simple python poetry package cheatsheet

| Command | Description | Example |
| --- | --- | --- |
| init | Initializes a new project with a `pyproject.toml` file. | `poetry init` |
| install | Installs dependencies listed in `pyproject.toml`. | `poetry install` |
| update | Updates dependencies to their latest versions. | `poetry update` |
| add | Adds a new dependency to the project. | `poetry add pendulum` |
| remove | Removes a dependency from the project. | `poetry remove requests` |
| show | Displays information about a package or its version. | `poetry show pandas` |
| build | Builds the project for distribution. | `poetry build` |
| publish | Publishes the project to a package repository. | `poetry publish` |
| config | Configures Poetry settings, such as repositories and environments. | `poetry config --add-repository https://example.com/repo` |
| run | Runs a command or script with the project's dependencies. | `poetry run python script.py` |
| shell | Opens an interactive shell with the project's dependencies. | `poetry shell` |
| check | Checks the project's dependencies for consistency and validity. | `poetry check` |
| search | Searches for packages on PyPI or other package repositories. | `poetry search pandas` |
| lock | Locks the project's dependencies to their current versions. | `poetry lock` |
| version | Displays Poetry's version number. | `poetry --version` |
