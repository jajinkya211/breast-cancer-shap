## File Descriptions

- **notebooks/SHAP.ipynb** — Reproducible end-to-end workflow: data loading (sklearn breast cancer), preprocessing, baselines (LogReg/XGBoost/MLP), evaluation (accuracy, ROC-AUC, CV), and SHAP-based explainability (global/instance-level plots). Seeded where possible.

- **docs/SHAP-Colab.pdf** — Printable export of the notebook for quick review and sharing. Regenerate this after substantial changes to keep PDF results aligned with the notebook.

- **requirements.txt** — Minimal pip dependencies for CPU execution (NumPy/Pandas/Scikit-learn/XGBoost/SHAP/plotting/Jupyter). PyTorch is intentionally not pinned here; follow the official selector for your OS/GPU.

- **environment.yml** — Conda environment with CPU-only PyTorch from the `pytorch` channel. Recommended for a one-command, reproducible setup.

- **.gitignore** — Ignores Python bytecode, Jupyter checkpoints, virtual environments, OS files, and typical data/output directories to keep the repo clean.

- **LICENSE** — Legal terms for reuse. This project uses the permissive MIT License, allowing commercial and non-commercial reuse with attribution. No warranty is provided.

- **CONTRIBUTING.md** — How to propose changes (fork → branch → PR), expectations (run the notebook end-to-end), and how to update dependency files when adding/removing packages.

- **CITATION.cff** — Enables “Cite this repository” on GitHub. If you mint a DOI (e.g., via Zenodo), add it here; you can also add ORCID and preferred citation details.

- **README.md** — Project overview, methods, environment setup, usage instructions, repository structure, and acknowledgements. Start here.
