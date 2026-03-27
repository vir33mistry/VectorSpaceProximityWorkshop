# VectorSpaceProximity Assignment

This folder contains the final completed notebook for the Vector Space Proximity assignment.

## Files

- `VectorSpaceProximity_final.ipynb` → final completed notebook
- `VectorSpaceProximity_updated.ipynb` → earlier completed version
- `VectorSpaceProximity.ipynb` → original assignment notebook

## What this notebook does

The notebook completes the end-to-end Vector Space Proximity challenge by building a small Information Retrieval system on a real text corpus.

It includes:

- loading a real corpus using the **20 Newsgroups** dataset from `sklearn.datasets`
- text preprocessing
- tokenizer
- normalization
- stop-word removal
- stemming
- term-document incidence matrix
- term frequency
- log-frequency weighting
- document frequency
- inverse document frequency
- TF-IDF weighting
- cosine similarity retrieval
- 5 information needs / queries
- comparison of **Binary**, **Raw TF**, and **TF-IDF**
- relevance explanations for retrieved documents
- evaluation for 3 queries
- confusion matrix
- precision, recall, F1-score
- Precision@10
- Average Precision (AP)
- Reciprocal Rank (RR) and MRR
- Cohen's Kappa demonstration
- reflection answers and simple talking points

## How the corpus is loaded

The corpus is loaded with:

```python
from sklearn.datasets import fetch_20newsgroups
```

The notebook uses selected categories from the **20 Newsgroups** dataset.

Important points:

- the corpus is **not required** to be stored as a `.csv` file
- it is fetched from **scikit-learn**
- on the first run, scikit-learn may download the dataset and cache it locally
- the notebook also includes a step to **export the selected corpus to a CSV file** for easier inspection

## Selected categories

The notebook uses these six categories:

- `sci.space`
- `rec.sport.hockey`
- `comp.graphics`
- `talk.politics.mideast`
- `sci.med`
- `rec.autos`

## How to run

1. Open the project folder in VS Code or Jupyter.
2. Make sure Python and Jupyter are installed.
3. Install the required packages if they are not already installed.
4. Run the notebook from top to bottom.

## Suggested packages

Install these packages in your environment if needed:

```bash
pip install numpy pandas matplotlib scikit-learn nltk jupyter
```

## Important note before running

Because the notebook uses `fetch_20newsgroups`, the first run may need internet access to download the dataset if it is not already cached on your system.

## Output

When you run the notebook, it will also create a CSV export file named:

- `20newsgroups_selected_corpus.csv`

This CSV export is an extra supporting file.  
The assignment itself is still correctly based on the scikit-learn corpus source.

## Final note

This final notebook is designed so the assignment questions are covered clearly, and the markdown talking points are written in simple language for class explanation.

## Authors

1) Param Rasaniya, Student ID: 9086095  
2) Viraj Mistry, Student ID: 9088985
