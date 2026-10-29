# EdTech App Market Analysis | Python, SQL & Power BI

An exploratory analytics portfolio project examining a **sample of education-related mobile apps** using prepared CSV data, Python visualizations, K-Means clustering, SQL reporting queries and a Power BI report.

**Important:** This is a historical sample and an analytical exercise, not a live view of Google Play, current app rankings or an official industry survey.

## Questions explored

- Which apps and developers have the largest observed install counts?
- How do review counts and app scores vary?
- How do average scores compare between apps with and without advertising?
- Which Android version values appear most often in the dataset?
- How do apps cluster when standardized installs, reviews and scores are used?

## Project assets

| Folder | Purpose |
|---|---|
| [data/](data/) | Cleaned app dataset and precomputed cluster result CSV |
| [notebooks/Edtech.ipynb](notebooks/Edtech.ipynb) | Data exploration, plots and K-Means |
| [sql/SQL_Insights.sql](sql/SQL_Insights.sql) | SQL Server queries using imported table `edtech_Final` |
| [powerbi/EdTech_Dashboard.pbix](powerbi/EdTech_Dashboard.pbix) | Power BI Desktop dashboard |
| [outputs/](outputs/) | CSV extracts for popular apps, Android versions, developers and ad comparison |
| [docs/](docs/) | Original documentation, setup and known limitations |
| [docs/legacy/Dashboard.twb](docs/legacy/Dashboard.twb) | Archived Tableau workbook **about external employee data**, not the EdTech app dataset |

## Reproducing Python analysis

From the repository root:

```bash
python -m venv .venv
# Activate the virtual environment for your OS
pip install -r requirements.txt
jupyter lab
```

Open [the notebook](notebooks/Edtech.ipynb). The input has been corrected to `data/edtech_cleanedData_Final.csv`—a file actually committed here. Running the final export cell updates `data/edtech_with_clusters.csv` locally. Keep the notebook's working directory at the repository root.

## SQL and dashboard

Import [the prepared CSV](data/edtech_cleanedData_Final.csv) as an appropriately typed `edtech_Final` table in SQL Server, then run [the SQL query examples](sql/SQL_Insights.sql). Open [the PBIX](powerbi/EdTech_Dashboard.pbix) in Power BI Desktop, update the data connection and verify reported metrics; no live report link is certified here.

## Limitations and integrity

The original notebook expected `edtech_Final.csv`, which was absent, and the repository's `Dashboard.twb` describes an unrelated SQL Server employee datasource. Both issues are documented rather than misrepresented as a reproducible EdTech dashboard. Model clusters are descriptive groups, not a causal explanation of success. Data and clustering outputs have not been rerun and reconciled here.

The GitHub workflow validates JSON/CSV structure and required file presence; it **does not** execute the notebook, SQL Server queries or Power BI refresh. See [quality and setup notes](docs/REPRODUCTION.md).

**Maintainer:** [bhagabatabrahma0106-dotcom](https://github.com/bhagabatabrahma0106-dotcom)
