# Titanic Data Cleaning

Starter notebook for cleaning the Titanic passenger dataset (891 rows, 12 columns). Setup and data loading are in place; the cleaning steps are still to do.

## Files

| File | Description |
|---|---|
| `clean.ipynb` | Starter notebook: imports (NumPy, Matplotlib, pandas) and CSV load |
| `Titanic-Dataset.csv` | Raw Titanic data |

## Dataset

Columns: `PassengerId`, `Survived`, `Pclass`, `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Ticket`, `Fare`, `Cabin`, `Embarked`.

| Issue | Count |
|---|---|
| Missing `Age` | 177 |
| Missing `Cabin` | 687 |
| Missing `Embarked` | 2 |
| Duplicate rows | 0 |

Overall survival rate: 38.4%.

## Status

- [x] Load data
- [ ] Handle missing values (`Age`, `Cabin`, `Embarked`)
- [ ] Fix dtypes and standardise text
- [ ] EDA and feature engineering

## Run it

```bash
git clone https://github.com/Nirmalya625/data_cleaning-and-eda-for-data-analysis.git
cd data_cleaning-and-eda-for-data-analysis
pip install pandas numpy matplotlib jupyter
jupyter notebook clean.ipynb
```

The notebook loads the CSV from a local Windows path (`C:\Users\LENOVO\...`) and fails with `FileNotFoundError` elsewhere. Change it to `pd.read_csv("Titanic-Dataset.csv")` before running.

## Author

**Nirmalya** – [GitHub](https://github.com/Nirmalya625)
