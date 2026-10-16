# Stock Market Project

A Python project that experiments with neural networks for stock market prediction.

## Goal
Train a neural network / machine learning model to predict the stock market as accurately as possible, using the best AI engineering methods and techniques available. Later, add a simple web page interface to show the model's results and training progress.

- Dataset: Kaggle `borismarjanovic/price-volume-data-for-all-us-stocks-etfs`, loaded via `kagglehub` (per-ticker CSV files in `Stocks/` and `ETFs/`; columns `Date,Open,High,Low,Close,Volume,OpenInt`; some files are empty)
- Evaluate honestly: split train/test by time (no shuffling across dates, no future data leaking into features) and always compare against a naive baseline (e.g. "tomorrow = today")

## Structure
- `Neural_Network.ipynb` — main Jupyter notebook with the model work

## Conventions
- Python, run in Jupyter notebooks
- Keep data files, model checkpoints and virtual environments out of git (see `.gitignore`)
- Don't commit API keys or credentials; put them in a `.env` file

## Working with Claude
- Do NOT change anything in this folder (files, notebooks, environments, installed packages) unless the user explicitly approves it or asks for it.
- For any request, propose ideas and suggested changes first, explaining what the user could do, and wait for approval before acting.
