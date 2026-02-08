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

```text
.
├── data/
│   ├── portfolio.csv
│   ├── profile.csv
│   └── transcript.csv
├── notebooks/
│   └── starbucks_restructured.ipynb
├── requirements.txt
└── README.md
```

1) macOS/Linux:
```
python3 -m venv .venv
source .venv/bin/activate
```
Windows (PowerShell):
```
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