# Unified Poetry Cheatsheet
This cheatsheet encompasses commands for package management and environment management:

| Example | Description |
| --- | --- |
| `poetry --help` | Displays help information for all commands. |
| `poetry --version` | Displays the current version of Poetry. |
| `poetry --verbose` | Increases verbosity level, `-v` for normal, `-vv` for more verbose, and `-vvv` for debug output. |
| `poetry --quiet` | Suppresses all output messages. |
| `poetry --ansi` | Forces ANSI output. |
| `poetry --no-ansi` | Disables ANSI output. |
| `poetry --no-interaction` | Disables any interactive prompts. |
| `poetry --no-plugins` | Disables plugins for the command run. |
| `poetry --no-cache` | Disables cache use during command execution. |
| `poetry --directory=DIRECTORY` | Sets the directory for commands, default is current directory. |
| `poetry new my-package` | Creates a new Python project with a standard directory structure. |
| `poetry new my-folder --name my-package` | Specifies a different package name than the directory. |
| `poetry new --src my-package` | Uses a `src` layout for the project structure. |
| `poetry new --src --name my.package my-package` | Sets up a project with namespace packages inside a `src` directory. |
| `poetry init` | Starts an interactive setup to create a `pyproject.toml` file. |
| `poetry install` | Installs dependencies from `pyproject.toml` and creates a `poetry.lock` file if absent. |
| `poetry install --without test,docs` | Excludes specific dependency groups during installation. |
| `poetry install --with test,docs` | Includes optional dependency groups during installation. |
| `poetry install --only test,docs` | Installs only specified dependency groups. |
| `poetry install --only-root` | Installs only the project package, no dependencies. |
| `poetry install --sync` | Synchronizes the environment exactly with the lock file. |
| `poetry install --extras "mysql pgsql"` | Installs the project with specified extras. |
| `poetry install --no-root` | Skips installation of the project package itself. |
| `poetry install --compile` | Compiles Python source files to bytecode during installation. |
| `poetry update` | Updates all project dependencies to their latest versions and updates `poetry.lock`. |
| `poetry update requests toml` | Updates specific packages within the constraints of `pyproject.toml`. |
| `poetry add requests` | Adds a new dependency to `pyproject.toml` and installs it. |
| `poetry add requests@^2.0.5` | Adds a dependency with a version constraint. |
| `poetry add git+https://github.com/sdispater/pendulum.git` | Adds a git repository as a dependency. |
| `poetry add --editable ./my-package/` | Adds a local package in editable mode. |
| `poetry remove requests` | Removes a dependency from the project. |
| `poetry show pandas` | Displays information about a package or its version. |
| `poetry build` | Builds the project into distributable archives. |
| `poetry publish` | Publishes the package to a package repository. |
| `poetry config --add-repository https://example.com/repo` | Configures Poetry settings, such as repositories and environments. |
| `poetry run python script.py` | Runs a command within the project's virtual environment. |
| `poetry shell` | Spawns a shell with the project's virtual environment activated. |
| `poetry check` | Checks the validity of the `pyproject.toml` file and the consistency of the lock file. |
| `poetry search pandas` | Searches for packages in the configured repositories. |
| `poetry lock` | Locks the project dependencies without installing them. |
| `poetry export -f requirements.txt --output requirements.txt` | Exports dependencies to a `requirements.txt` file. |
| `poetry env use /full/path/to/python` | Sets the specific Python version for the current project. |
| `poetry env use python3.7` | Uses the Python executable in your PATH. |
| `poetry env use 3.7` | Uses a minor Python version specified. |
| `poetry env use system` | Uses the system's default Python, deactivating the virtual environment. |
| `poetry env info` | Displays information about the currently activated virtual environment. |
| `poetry env info --path` | Shows the path to the virtual environment. |
| `poetry env info --executable` | Shows the path to the python executable in the virtual environment. |
| `poetry env list` | Lists all virtual environments associated with the project. |
| `poetry env list --full-path` | Displays the full path to the environments. |
| `poetry env remove /full/path/to/python` | Removes specified virtual environments. |
| `poetry env remove python3.7` | Removes environments by specifying executable version. |
| `poetry env remove 3.7` | Removes environments by specifying minor version. |
| `poetry env remove python3.6 python3.7 python3.8` | Deletes multiple environments at once. |
| `poetry env remove --all` | Deletes all associated virtual environments at once. |

