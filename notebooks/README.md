# Notebooks and execution order

## Preserved preliminary notebooks

- `01_setup.ipynb`: original environment setup experiment. Kept unchanged for traceability.
- `02_aila_retrieval_experiments.ipynb`: original AILA experiments. Kept unchanged; contains repeated setup and exploratory cells.

These notebooks are historical/preliminary work, not the clean IL-TUR pipeline. Do not assume their outputs are final research results.

## New research notebooks

New IL-TUR notebooks will be added only after Phase 1 verifies the dataset's real structure and evaluation format. The planned sequence is:

1. Environment setup
2. IL-TUR dataset verification
3. Data preprocessing
4. BM25 baseline
5. Semantic retrieval
6. Issue-aware retrieval
7. Explainability
8. Faithfulness evaluation
9. Stability evaluation
10. Final comparison

Each notebook should have a clear purpose, minimal repeated setup, documented inputs and saved outputs. Keep secrets out of notebook cells and outputs.
