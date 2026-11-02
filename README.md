# STAT 386: Visualization demo

The instructor notebooks start with the most basic working plot and add one improvement at a time. Student exercises and extra examples are separate files.

## Get started

1. Unzip the whole project and open this folder in VS Code with its Python and Jupyter extensions.
2. Run `uv sync` in the terminal. The retained project configuration uses Python 3.13. The first dependency installation requires internet access.
3. Open a notebook and select the Python interpreter from this folder's `.venv` as its kernel.
4. Keep the notebook working directory at the repository root, where `data/` is visible. Run cells in order within each notebook.

Every notebook loads its own data, so no other notebook needs to be run first. The revised notebooks use a local CSV and need no dataset downloads. No Streamlit installation is needed for the teaching notebooks.

## Instructor teaching sequence

| File | Teaching progression |
|---|---|
| [0-anscombe.ipynb](0-anscombe.ipynb) | Optional opener: similar summaries, different structures |
| [1-matplotlib.ipynb](1-matplotlib.ipynb) | Basic scatter -> labels -> log scale -> mark settings -> two panels -> save |
| [2-seaborn.ipynb](2-seaborn.ipynb) | Basic scatter -> hue -> Matplotlib refinements; basic boxplot -> individual observations |
| [3-plotly.ipynb](3-plotly.ipynb) | Basic scatter -> log scale -> hover names -> color -> labels -> HTML; brief Streamlit connection |

The main notebooks are complete instructor demonstrations with no student coding blanks. Each library also includes one clearly labeled advanced showcase before its closing comparison: Matplotlib symbols and an annotation, Seaborn facets for two years, and a Plotly animation with population-sized bubbles colored by country. The basic teaching sequence remains unchanged. Each library closes with its strengths and tradeoffs. See [INSTRUCTOR_GUIDE.md](INSTRUCTOR_GUIDE.md) for the comparison, discussion notes, and suggested stopping points.

## Separate student and extension files

| File | Purpose |
|---|---|
| [practice-1-guided.ipynb](practice-1-guided.ipynb) | Matplotlib revision, Seaborn distribution comparison, Plotly investigation, and tool choice |
| [practice-2-eda.ipynb](practice-2-eda.ipynb) | Independent question, plot, partner critique, revision, and caption |
| [extra-examples.ipynb](extra-examples.ipynb) | Baselines, country trends, counts versus means, facets, bins, heatmaps, bubbles, animation, and consistent color mappings |
| [instructor-solutions.ipynb](instructor-solutions.ipynb) | Worked practice examples and discussion answers |

Do not feel obligated to cover every optional example in class. Student-only copies can omit the instructor guide and solutions.

## Shared data and exports

Gapminder is a historical teaching extract with 142 countries and 12 observations per country from 1952 to 2007. Cross-sectional plots explicitly use 2007; one point is one country. See [data/README.md](data/README.md) for units, provenance, and limits.

Examples save generated figures in `outputs/`. Plotly HTML preserves browser interaction and can be linked from a GitHub Pages site. Streamlit can build an app around a Plotly figure when controls need to run Python calculations; the brief illustration is in the Plotly teaching notebook.

## Earlier materials and validation

The five originally uploaded notebooks remain unchanged in `reference/original/`. They are historical material outside the current sequence and still contain their original downloads and unfinished cells. No tornado-data download is needed by the revised materials.

The original dependency constraints and lockfile are retained. [VALIDATION.md](VALIDATION.md) records what was executed and the remaining interactive-rendering checks.
