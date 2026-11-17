# Notebooks and execution order

## Start here

- `00_environment_setup.ipynb`: the canonical Google Colab setup notebook. Mounts Drive, creates the standard project folders, installs dependencies and checks the runtime.

## Preserved preliminary notebooks

- `01_setup.ipynb`: original setup experiment, retained unchanged for traceability. Do not use it as the current setup guide.
- `02_aila_retrieval_experiments.ipynb`: original AILA experiments, retained unchanged. It contains exploratory and preliminary work, not the clean IL-TUR pipeline. Its semantic evaluation needs review because the notebook records query-length truncation diagnostics.

AILA results must not be presented as IL-TUR results.

## Planned IL-TUR research sequence

The following notebooks will be added after Phase 1 verifies the dataset's actual structure, query format, candidate judgments, relevance labels, annotations and licence:

1. `01_iltur_dataset_verification.ipynb`
2. `02_data_preprocessing.ipynb`
3. `03_bm25_baseline.ipynb`
4. `04_semantic_retrieval.ipynb`
5. `05_issue_aware_retrieval.ipynb`
6. `06_explainability.ipynb`
7. `07_faithfulness_evaluation.ipynb`
8. `08_stability_evaluation.ipynb`
9. `09_comparison_and_analysis.ipynb`

Each notebook should have one main responsibility, minimal repeated setup, documented inputs and saved outputs. Keep secrets and restricted data out of notebook cells and outputs.
