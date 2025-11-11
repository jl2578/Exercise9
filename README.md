## Exercise 9: Quantitative Reactivity Case Study

This repository contains the Jupyter notebook and supporting data for **Exercise 9** of your course. The notebook explores behavioural and functional magnetic resonance imaging (fMRI) data related to task‑evoked reactivity in the nucleus accumbens (NAcc).

### Contents

- **`Exercise9.ipynb`** – the main Jupyter notebook students will work through.
- **`data/e9_qreact_behavior_min.csv`** – summary behavioural data for the quantitative reactivity task.
- **`data/e9_task_qreact_roi_betas.csv`** – region‑of‑interest (ROI) beta estimates for the quantitative reactivity task.
- **`.devcontainer/`** – development‑container configuration for a reproducible coding environment.
- **`requirements.txt`** – Python package dependencies used in the notebook.

### Getting Started

To run the notebook locally, create a Python virtual environment and install the required packages:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook Exercise9.ipynb
```

Alternatively, you can open this repository in VS Code using Dev Containers. The `.devcontainer` folder defines a container with Python, Jupyter and the GitHub Copilot extension preinstalled. When the container is built, VS Code will automatically install the dependencies from `requirements.txt`. Once running, you can open and execute `Exercise9.ipynb` in the container without affecting your host system.

### Data Files

The notebook expects two CSV files stored under the `data/` directory:

- `e9_qreact_behavior_min.csv` contains trial‑level behavioural measures (such as reaction times). Each row corresponds to a single observation.
- `e9_task_qreact_roi_betas.csv` contains beta weights derived from ROI analyses of fMRI data. Columns represent brain regions and rows correspond to subjects or conditions.

These files are included here so the notebook can run offline. If you update these data sets for your own analysis, ensure that the file paths in the notebook remain correct.

### Licence

This repository is intended for educational purposes. If you wish to reuse or modify the material outside of the course, please consult your instructor regarding the applicable licence terms.
