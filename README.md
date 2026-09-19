# ML From Scratch

Core machine learning algorithms implemented from scratch in NumPy, with the
math written up and every implementation tested against scikit-learn.

**Why this exists:** using `.fit()` is easy, and understanding what happens
inside it is the point. Each algorithm here has a math note, a NumPy-only
implementation, a test against scikit-learn, and a notebook on a real dataset.
scikit-learn is used only for comparison, never inside the algorithms.

## Status

| Algorithm | Math note | Implementation | Test vs sklearn | Notebook | Result |
|---|---|---|---|---|---|
| Linear regression | not started | not started | not started | not started | - |
| Logistic regression | not started | not started | not started | not started | - |
| K-nearest neighbors | not started | not started | not started | not started | - |
| Decision tree | not started | not started | not started | not started | - |

Update this table only when the work is committed.

## Results

| Algorithm | Dataset | My metric | scikit-learn metric |
|---|---|---|---|
| <fill in as you finish each> | | | |

## Repo structure

```
mlscratch/       algorithm implementations (NumPy only)
  metrics.py         MSE, R2, accuracy, precision, recall
  preprocessing.py   train/test split, standard scaler
tests/           checks that outputs match scikit-learn
notebooks/       demos on real datasets
docs/            one-page math notes per algorithm
```

## Run it

```bash
git clone https://github.com/<your-username>/ml-from-scratch.git
cd ml-from-scratch
pip install -r requirements.txt
pytest
```

## How each algorithm is built

1. Write the math note in `docs/` first: the model, the loss, the gradient and
   the update rule.
2. Implement it in `mlscratch/` with `fit(X, y)` and `predict(X)`.
3. Add a test that compares its output to scikit-learn on the same data.
4. Show it working in a notebook on a real dataset, with a loss curve.

## Datasets

Data files are not stored in this repo. Each notebook links to where its
dataset can be downloaded.

## Related

- [concept-diary](https://github.com/Somesh246-12/concept-diary): my daily
  ML concept log.