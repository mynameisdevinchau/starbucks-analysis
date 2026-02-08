# Starbucks Analysis

Starbucks distributes promotional offers to drive customer purchases, but it is not always clear which offers positive influence customer behavior. Some offers are viewed, some are completed quickly, and some are completely ignored. This project aims to evaluate the effectiveness of the different types of offers by tracking how customers move through the offer funnel (received → viewed → completed) and measuring where drop-off occurs. By linking offer events to customer attributes and timing, the project is going to try to identify which promotions perform best and which audiences respond most.

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

1. macOS/Linux:

```
python3 -m venv .venv
source .venv/bin/activate
```

Windows (PowerShell):

```
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install dependencies

```
pip install -r requirements.txt
```

3. Run the notebook

```
jupyter lab
```
