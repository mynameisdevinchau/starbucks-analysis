# Starbucks Analysis

A Jupyter notebook project that analyzes customer behavior on the Starbucks Rewards app, focusing on how different offers (type, duration, channels) move users through the funnel (received → viewed → completed), and what segments respond best.

## What’s inside

- **Exploratory analysis**
  - Distributions for key fields (age, income, membership tenure)
  - Offer mix and channel usage
  - Transaction patterns over time
- **Offer funnel + attribution**
  - Links offer events per customer and offer id
  - Measures view rate, completion rate, time-to-view, time-to-complete
  - Handles edge cases like duplicate receipts and events outside an offer window
- **Segment insights**
  - Breakdowns by demographics and membership tenure
  - Offer performance by type (BOGO/discount/informational) and channel

## Repo structure


The repository contains `data/`, `notebooks/`, and `requirements.txt` on the `main` branch. :contentReference[oaicite:1]{index=1}

## Data

This project expects the typical Starbucks Rewards app dataset used in the Udacity capstone-style project:
- `portfolio.json` (offer metadata: type, channels, duration, difficulty, reward)
- `profile.json` (customer demographics + membership date)
- `transcript.json` (events: offer received/viewed/completed + transactions)

Place them under `data/` if they aren’t already there.

> Note: If you publish this repo, double check you’re allowed to redistribute the raw dataset. If not, keep `data/` out of Git and add a small “how to obtain data” note instead.

## Setup

### 1) Create and activate a virtual environment

macOS / Linux:
```bash
python3 -m venv .venv
source .venv/bin/activate
```
```
Windows (Powershell)

python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2) Install dependencies
```
pip install -r requirements.txt
```

3) Run the notebook
```
jupyter lab
```
