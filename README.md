# Data-visualization-Using-Matplotlib

This collection demonstrates core plotting techniques using Matplotlib and Seaborn, with ready-to-run Jupyter notebooks and a small demo script. It's designed for learners and practitioners who want hands-on examples of common chart types, styling, and interactive workflows.

**Location**: `anaconda_projects/db/`

**Highlights**:
- **Concise notebooks** covering individual chart types (bar, pie, histogram, scatter, etc.).
- **Seaborn examples** showing statistical plots, heatmaps and dataset usage.
- **Interactive tips** for running plots inside Jupyter and enabling interactive backends.

**Prerequisites**

- Python 3.8+ (3.10 recommended)
- An environment manager such as `conda` or `venv`.
- Required packages: `matplotlib`, `seaborn`, `pandas`, `numpy`, `jupyter`.

Quick install (PowerShell):

```powershell
conda create -n viz python=3.10 -y; conda activate viz
pip install matplotlib seaborn pandas numpy jupyter ipympl
```

Notes:
- Install `ipympl` (`pip install ipympl`) to use the `%matplotlib widget` backend for interactive figures in Jupyter.

Project Structure

- `anaconda_projects/db/`
  - `01_introduction_Matplotlib.ipynb` — Matplotlib basics and first plots.
  - `02_Bar_Charts_in_Matplotlib.ipynb` — Bar chart patterns and styling.
  - `03_Pie_Charts_in_Matplotlib.ipynb` — Pie chart generation and best practices.
  - `04_Stack_Plots_in_Matplotlib.ipynb` — Stacked area/line plots.
  - `05_Histograms_in_Matplotlib.ipynb` — Distributions and histogram options.
  - `06_Scatter_Plots_in_Matplotlib.ipynb` — Scatter plots and visual encodings.
  - `07_Subplots_in_Matplotlib.ipynb` — Arranging multiple axes and figure layouts.
  - `08_Introduction_to_Seaborn.ipynb` — Seaborn concepts and simple examples.
  - `09_Basic_Plot_Types_in_Seaborn.ipynb` — Lineplot, scatter, bar, boxplot, heatmap examples and pivoting.
  - `matplotlib_demo.py` — A small script demonstrating programmatic plotting outside notebooks.

Notebook Summaries (what you'll learn)

- **01_introduction_Matplotlib.ipynb** — Figure and axis construction, basic lines, labels, and saving figures.
- **02_Bar_Charts_in_Matplotlib.ipynb** — Creating grouped and stacked bars, error bars, and color palettes.
- **03_Pie_Charts_in_Matplotlib.ipynb** — Slice labels, exploded slices, and accessibility considerations.
- **04_Stack_Plots_in_Matplotlib.ipynb** — Creating stacked area charts and annotating cumulative values.
- **05_Histograms_in_Matplotlib.ipynb** — Binning strategies, KDE overlays, and comparing distributions.
- **06_Scatter_Plots_in_Matplotlib.ipynb** — Point size, color encoding, regression overlays, and jittering.
- **07_Subplots_in_Matplotlib.ipynb** — `plt.subplots()` usage, shared axes, and constrained layout.
- **08_Introduction_to_Seaborn.ipynb** — High-level APIs for statistical plots and dataset loading.
- **09_Basic_Plot_Types_in_Seaborn.ipynb** — Examples using `tips` and `flights` datasets: lineplot, scatterplot with `hue`, barplot, boxplot, heatmap; includes pivoting data for heatmaps.

How to use

- To explore interactively, open the folder in Jupyter Notebook or JupyterLab:

```powershell
cd "d:\Data Science\Matplotlib\anaconda_projects\db"
jupyter lab
```

- In each notebook, enable inline rendering with `%matplotlib inline` or interactive widgets with `%matplotlib widget`.

- To run the demo script:

```powershell
python "d:\Data Science\Matplotlib\anaconda_projects\db\matplotlib_demo.py"
```

Interactive Tips

- Use `%matplotlib widget` for zoomable, pannable figures in Jupyter (requires `ipympl`).
- For Seaborn plots, pass `palette=` and `style=` options to experiment with different aesthetics.
- When presenting results in slides or reports, export figures with `fig.savefig('figure.png', dpi=300, bbox_inches='tight')`.

Suggested Exercises

- Recreate a style by changing `plt.style.use('seaborn-darkgrid')` and comparing outputs.
- Add error bars to bar charts and explore `sns.barplot(..., ci='sd')`.
- Convert the `flights` dataset pivot to a normalized heatmap (percent of yearly total).

Contributing

If you'd like to add examples or improvements:

- Fork the repo (or copy the folder), add or refine a notebook, and submit a pull request with a short description of the change.
- Keep notebooks focused and small — each notebook should teach one or two concepts.

License & Attribution

This collection references example datasets provided by Seaborn (`tips`, `flights`). Credit Seaborn and Matplotlib when reusing examples. Add a license file at the repo root if you intend to publish or share broadly.

Questions or Changes

Open an issue or message the repository owner with suggestions. After reviewing, we'll incorporate improvements, add a `requirements.txt`, or provide a conda `environment.yml` if needed.

---

Created from the examples inside `anaconda_projects/db/` to provide a clear, runnable learning path for Matplotlib and Seaborn visualizations.
