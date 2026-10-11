# Hands-On Machine Learning — Personal Study Notebooks

A discussion-led study companion to *Hands-On Machine Learning with Scikit-Learn and PyTorch* by Aurélien Géron.

## Working rule

Notes, equations, figures and Python experiments are added **only after we have discussed and understood a topic**. Chapter notebooks initially contain only their headings. We do not automatically summarize or copy the textbook.

## Folders

- `chapters/ch01-...` to `chapters/ch19-...` — one Jupyter notebook per chapter; notes, math and runnable code together.
- `data/` — chapter datasets when needed. Ignored by Git by default; no book downloads included.
- `figures/` — images and figures we create while studying; tracked by Git.

No `scripts/` folder initially. If we write useful code that needs to be shared between chapters, we'll add it then. Likewise, appendices can be added only if we decide to study them.

## WSL / Linux setup

From the project directory (install [uv](https://docs.astral.sh/uv/) first, if needed):

```bash
uv sync
uv run jupyter lab
```

Then open `chapters/ch01-the-machine-learning-landscape/ch01.ipynb`. This project targets Python 3.12. PyTorch is intentionally not installed yet; we'll add it when required.

## Our study workflow

1. Read a topic in the hard-copy book.
2. Discuss the concept, intuition and required mathematics.
3. Write concise notes in our own words, with small examples.
4. Add and run Python experiments in the same notebook.
5. Commit finished updates to Git.

## Initialize Git locally

```bash
git init -b main
git add .
git commit -m "chore: initialize ML study notebooks"
```

Create a private remote GitHub repository and push when ready. Do not commit the EPUB or proprietary textbook material.
