# Charts - Python Visualisation Course

Learning materials for an introductory data visualisation course using Python, Pandas, Matplotlib, and Seaborn.

| File | Contents |
|---|---|
| `01_basic_charts.py` | Line charts, scatter plots, linear/quadratic fits, actual vs predicted |
| `02_bar_charts.py` | Bar charts, step-by-step beautification, misleading chart techniques |
| `03_advanced_plots.py` | Count, histogram, KDE, strip, swarm, box, violin, jointplot, pairplot, heatmap |
| `04_quiz.py` | Five graded exercises on the Iris dataset with LLM prompts and reference solutions |

Each `.py` file is a VS Code Interactive Python notebook (`# %%` cell format).
Matching `.ipynb` files are also provided for use in JupyterLab or classic Jupyter.

## Installation

```bash
conda create --name charts python=3.13
conda activate charts
pip install -r requirements.txt
```

## Running

### With JupyterLab (recommended)

Open the `.ipynb` file for any topic in JupyterLab:

```bash
jupyter lab
```

Then navigate to the file and run cells with **Shift+Enter**, or use **Run → Run All Cells**.

### Alternative: VS Code Interactive window

Open the corresponding `.py` file in VS Code with the Python extension installed.
Run individual cells with **Shift+Enter**, or use **Run All Cells** from the toolbar.
The interactive output appears in the Python Interactive panel on the right.

---

## What is Conda and why are we using it?

**Conda** is a tool that manages Python installations and the libraries that come with them.
Think of it as an app store for Python packages — it lets you install, update, and remove
libraries like Pandas or Matplotlib with a single command.

### What is a conda environment?

A **conda environment** is an isolated box that contains its own Python version and its own
set of installed libraries. You can have many environments on the same computer, each with
completely different setups, and they will never interfere with each other.

A simple analogy: imagine each project has its own toolbox. You keep the tools for one
project separate from another so that swapping a tool in one box never breaks anything in
another.

### Why do we use environments?

- **Avoid conflicts.** Different projects often need different versions of the same library.
  Without environments, installing a new version for one project can silently break another.
- **Reproducibility.** An environment can be described in a `requirements.txt` file, so
  anyone can recreate the exact same setup on a different machine with one command.
- **Clean uninstall.** When a project is finished, you simply delete the environment and
  nothing is left behind on your system.