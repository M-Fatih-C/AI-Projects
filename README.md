# Machine-learning notebook archive

An educational/research collection of **33 notebooks**: 32 numbered experiment
folders plus the root `Untitled16.ipynb`. It includes vision, speech/text,
tabular analysis, neural-network exercises and competition modeling. Historical
folder names are preserved; several describe the content inaccurately.

## Finding an experiment

[Source-based catalogue](docs/EXPERIMENT_CATALOG.md) gives each notebook a concrete
subject, observed libraries/model symbols and external artefact references.
Examples: folder 17 is speech-emotion work, 24 is an ant-detection experiment,
29 uses YouTube comments/LSTM, and 31 is an incomplete pose/gesture exercise.
These are independent learning experiments, not one reproducible application.

## Running a notebook

Use a dedicated environment for the selected experiment. The root requirements
list is an inventory starting point; it does not establish a mutually compatible
environment for all notebooks. Read notebook installation cells before executing
them: some install/uninstall packages or use Colab shell commands and Drive paths.

```bash
python3.12 -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
python -m pip install jupyter
jupyter notebook
```

Then supply the selected notebook's authorized dataset and trusted model files.
Kaggle/YouTube credentials must be configured privately; never replace placeholders
with committed keys. Model downloads, GPU memory, external images/audio and local
CSV/XLSX paths differ by experiment. Missing files mean a notebook is not ready
to run from a clean clone.

## Validation and privacy

The audit inspected notebook JSON and source cells without executing datasets,
training or external API calls. Static checks found a syntax error (`data[]`) and
an incorrect classifier import in notebook 31. There is no shared automated test
suite or current comparable benchmark. Preserved output charts/metrics are historical
artefacts; no fresh accuracy or performance result is claimed.

Notebook 18 references health-research data and retains aggregate outputs; owner
review of disclosure rights and re-identification risk remains necessary. Colab
metadata and other outputs may contain names/identifiers. No output/history was
automatically deleted, and the audit is not a privacy clearance for publication.
Use synthetic examples and keep private datasets, credentials and patient/customer
records outside Git. Any overlap with standalone competition repositories is
documentary context, not authorization to merge/delete archives.


## License and contact

See the existing [MIT license](LICENSE). Author: [Muhammet Fatih Çetintaş](https://github.com/M-Fatih-C).
