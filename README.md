# Terputer transcriptomics example

[Open this example in GitHub Codespaces](https://codespaces.new/Terpedia/terpedia-transcriptomics-demo?quickstart=1)

This public Codespace shows Terputer's notebook editor, Python execution, research chat interface, and a reproducible transcriptomics case study. The included [executed notebook](notebooks/terputer-transcriptomics.ipynb), [white paper](research/transcriptomics/white-paper.md), and [critical review](research/transcriptomics/critical-review.md) examine terpene exposure and context-specific signaling. Pinned source inputs and derived tables are under `research/transcriptomics/`.

The Codespace config installs Node.js and Python dependencies, starts Terputer and its Python kernel, and opens the private forwarded app port. In the app, select **Open repo notebook** and choose `terputer-transcriptomics.ipynb` to inspect the complete analysis. You can also open the notebook in VS Code's Jupyter editor. Run cells in your own Codespace and compare the output with the saved results.

The notebook and local Python kernel work without credentials. To use the in-app research agent, add `TERPUTER_OPENROUTER_API_KEY` as a Codespaces secret and restart the app. Terpedia Knowledge search additionally needs `TERPEDIA_KNOWLEDGE_API_KEY`. No secrets are included in this repository. The notebook's input data and outputs are provided so the published conclusions can be inspected without those services.

Terputer is a research workspace, and generated analyses require human review before scientific use. See the white paper's limitations and the critical review for the evidence boundaries.

## Local startup

```sh
npm ci
python -m pip install -r requirements.txt
bash .devcontainer/start.sh
```
