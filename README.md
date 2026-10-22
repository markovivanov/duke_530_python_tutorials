# Python for a fitness app

Nine introductory, 60-minute notebook workshops for master's students with mixed programming backgrounds. Each lesson starts with a concrete fitness app feature and assumes a beginner pace.

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

## Additional class material

[Carless: Denver neighborhood EDA](CLASS/denver_airbnb_eda.ipynb) puts students on a product team building an app for trips without a rental car. It introduces pandas, trip filters, neighborhood prices and ratings, word clouds, walking/transit searches, qualitative coding, and an evidence-based shortlist. See the [class guide and dataset notes](CLASS/README.md) for the teaching route and setup.

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

You can also open the files in VS Code with notebook support and select this folder's `.venv` as the kernel, or upload an individual notebook to Google Colab. For week 7, keep or upload the accompanying `data/run_distances_km.txt` file in a folder named `data` under the runtime's working folder. Weeks 8 and 9 require Matplotlib in the selected kernel.

## How the lessons work

- Each notebook includes a feature introduction, learning goals, a suggested schedule, a prerequisite refresher, and guided examples.
- Markdown callout boxes introduce concepts and explain common mistakes.
- Every meaningful Python line has an inline comment; closing-only delimiters and blank lines are exempt.
- Every notebook ends with two short exercises. Exercise 1 is the core task; exercise 2 is optional reinforcement if time allows.
- Exercises include hints, expected results, and runnable starter cells. The starter cells deliberately leave work for the student and do not contain completed solutions.
- All profiles, goals, and activity records are fictional. Units are stated explicitly.
- Each notebook defines what it needs rather than relying on another notebook's kernel state.
- Saved example outputs allow learners to read the lessons before running them. Rerun cells to explore changes.

## Sample files and generated output

Week 7 reads [data/run_distances_km.txt](data/run_distances_km.txt), containing seven daily distances totaling 20.0 km. Keep the `data` folder beside the notebooks.

Its guided example creates `fitness_weekly_summary.txt` in the working folder. The second exercise asks students to create `fitness_exercise_note.txt`. Write mode replaces the contents of these generated files when rerun. Neither write targets the supplied input log.

## Teaching pace

Allow 5 minutes for the feature and recap, 15 for concepts, 15 for a guided example, 10 for small changes and discussion, 10 for exercises, and 5 for questions. Treat these times as flexible targets. If learners need more time, skip a secondary example or the second exercise and preserve time for practice.

The class lesson focuses on understanding and using a supplied `FitnessProfile`. The final session provides a guided assembly of familiar pieces. Students can attend after missing a session by using the included definitions and prerequisite explanations.

## Verification

All nine notebooks were executed in separate fresh Python kernels with isolated working folders. Checks covered expected numerical results and decision boundaries, reading and writing the week 7 files, valid notebook structure, inline comments on meaningful code lines, and two final exercise starter cells per notebook. All notebooks rendered to HTML successfully, and the four embedded chart outputs were visually checked. Exercise solutions remain for students to complete.
