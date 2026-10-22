# Python for a fitness app

## Open a lesson

| Week | Notebook | App feature |
|---|---|---|
| 1 | [Variables and data types](01_intro_variables_and_types.ipynb) | Record a run |
| 2 | [Functions](02_functions.ipynb) | Calculate running pace |
| 3 | [Classes and objects](03_classes_and_objects.ipynb) | Create a fitness profile |
| 4 | [Lists and dictionaries](04_lists_and_dictionaries.ipynb) | Keep a workout history |
| 5 | [Conditionals](05_conditionals.ipynb) | Respond to a step goal |
| 6 | [Loops](06_loops.ipynb) | Summarize a week of activity |
| 7 | [Reading and writing files](07_reading_and_writing_files.ipynb) | Save and reload a workout log |
| 8 | [Libraries and visualization](08_libraries_and_visualization.ipynb) | Chart recorded runs |
| 9 | [Putting it together](09_putting_it_together.ipynb) | Build a weekly activity summary |

The detailed course outline is in [TUTORIAL_PLAN.md](TUTORIAL_PLAN.md).

## Use the prepared local environment

A project-local `.venv` has been prepared on this computer. From this workshop folder, launch JupyterLab with:

```sh
.venv/bin/python -m jupyterlab  # Start JupyterLab using the workshop's Python environment.
```

Open a notebook and select the Python 3 kernel. Run cells in order with the Run button or Shift + Enter. To restore the starting state, restart the kernel and run all cells.

## Set up another computer

Install Python 3 and open a terminal in the workshop folder. On macOS or Linux:

```sh
python3 -m venv .venv  # Create an isolated Python environment for the workshop.
.venv/bin/python -m pip install -r requirements.txt  # Install the notebook and charting tools.
.venv/bin/python -m jupyterlab  # Start JupyterLab from this folder.
```

On Windows, use the following commands in PowerShell:

```powershell
py -m venv .venv  # Create an isolated Python environment for the workshop.
.venv\Scripts\python.exe -m pip install -r requirements.txt  # Install the workshop tools.
.venv\Scripts\python.exe -m jupyterlab  # Start JupyterLab from this folder.
```

The notebooks use standard Python 3 syntax. Execution was checked with Python 3.14.6. The dependency ranges allow compatible versions to be selected for other supported Python installations.


