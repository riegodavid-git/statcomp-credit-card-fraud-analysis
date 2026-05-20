# Dataset

The credit-card-transactions dataset used in this project is approximately **354 MB** as a CSV (or ~224 MB as XLSX) — too large to commit directly to this GitHub repository.

## Source

**Credit Card Transactions Fraud Detection Dataset** by Kartik Shenoy on Kaggle:
https://www.kaggle.com/datasets/kartik2112/fraud-detection

## Download

```bash
# With the Kaggle CLI:
kaggle datasets download -d kartik2112/fraud-detection -p data/ --unzip
```

The notebook expects `data/credit card transactions.csv` (or rename as needed when reading).

## Schema (excerpt)

| Column | Description |
|---|---|
| `trans_date_trans_time` | Transaction timestamp |
| `cc_num` | Credit card number (hashed) |
| `merchant`, `category` | Merchant and product category |
| `amt` | Transaction amount |
| `first`, `last`, `gender`, `street`, `city`, `state`, `zip`, `lat`, `long` | Cardholder demographics & location |
| `dob`, `job`, `city_pop` | Cardholder profile |
| `merch_lat`, `merch_long`, `merch_zipcode` | Merchant location |
| `is_fraud` | **Target** — fraud label (0/1) |
