# Beyond Retrieval Accuracy: Evaluating Faithfulness and Stability of Explainable, Issue-Aware Indian Legal Precedent Retrieval

Research code and experiment tracking for an evaluation of Indian legal precedent retrieval systems.

## Research workflow

1. Verify the IL-TUR dataset: files, queries, candidate judgments, relevance labels, annotations and licence.
2. Set up the environment and project storage.
3. Preprocess queries and judgments; check missing, malformed and duplicate records.
4. Establish a BM25 baseline.
5. Implement semantic retrieval with Sentence Transformers.
6. Add issue-aware retrieval.
7. Produce evidence-grounded explanations for retrieved judgments.
8. Evaluate explanation faithfulness.
9. Evaluate ranking and explanation stability under query paraphrases and small edits.
10. Compare methods with retrieval metrics, error analysis and appropriate statistical tests.
11. Build an academic prototype.
12. Document results, limitations and contributions.

## Repository layout

- `notebooks/`: ordered, task-focused experiment notebooks.
- `src/`: reusable preprocessing, retrieval, evaluation and explanation code.
- `data/`: dataset location documentation. Raw and processed datasets are not committed.
- `results/`: experiment outputs and tables (small, non-sensitive files only).
- `reports/`: research notes and report material.

## Existing preliminary work

The two original notebooks are retained:

- `notebooks/01_setup.ipynb`: initial Google Drive setup and dependency checks.
- `notebooks/02_aila_retrieval_experiments.ipynb`: preliminary AILA experiments, including BM25, semantic chunking and diagnostics.

AILA results are preliminary and must not be presented as IL-TUR results. The semantic notebook records query-length truncation diagnostics; its semantic evaluation should not be treated as final without correcting and re-running affected experiments.

## Getting started

The intended environment is Google Colab with Google Drive for datasets and generated embeddings.

1. Open a notebook in `notebooks/`.
2. Install dependencies from `requirements.txt`.
3. Keep dataset files in Google Drive or another approved storage location.
4. Never commit private access tokens, credentials, large datasets or generated embedding arrays.

## Data and access

No dataset is included in this repository. Verify official dataset documentation, licence terms, access conditions and permitted uses before downloading or redistributing data. Do not assume access to IL-PCR/IL-PCSR or any other restricted collection.

## Reproducibility

Record dataset version and source, preprocessing choices, model name/version, chunking parameters, random seeds, evaluation split and metric definitions for every reported experiment. Keep development and test queries separate and do not tune on the test set.

## Project status

- [x] Initial repository and preliminary AILA notebooks preserved
- [x] Cleanup branch created
- [ ] IL-TUR dataset verification
- [ ] Reproducible environment and preprocessing
- [ ] BM25, semantic and issue-aware experiments
- [ ] Faithfulness and stability evaluation
- [ ] Prototype and final report
