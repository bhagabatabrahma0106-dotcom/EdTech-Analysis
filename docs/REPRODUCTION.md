# EdTech reproduction and quality notes

## File provenance
- Input: [cleaned CSV](../data/edtech_cleanedData_Final.csv). The original raw `edtech_Final.csv` is absent.
- Output: [cluster-labelled CSV](../data/edtech_with_clusters.csv), plus read-only CSV summaries in `outputs/`.
- Notebook: [Edtech.ipynb](../notebooks/Edtech.ipynb) now reads the committed cleaned dataset and exports to a committed path.
- Tableau: the [legacy workbook](legacy/Dashboard.twb) refers to a separate employee database, not EdTech app data. Do not use it as proof of Tableau EdTech visuals.

## Prerequisites
- Python 3.10+ with pandas, matplotlib, seaborn, scikit-learn and JupyterLab
- SQL Server for T-SQL insights
- Power BI Desktop for the dashboard file

## Validation
1. Run Jupyter from the repository root to resolve the `data/` paths.
2. Verify column types and null counts; installs/reviews can be highly skewed.
3. For K-Means, inspect the effect of scaling, seed choice, number of clusters and outliers. A cluster index (0/1/2) has no intrinsic low/medium/high meaning.
4. Compare generated CSV outputs with the committed versions before replacing them.
5. Inspect PBIX source and visuals with Power BI Desktop. The workbook, notebook outputs and SQL have not been end-to-end verified here.
6. Treat reported app installs and ratings as a historic sampled dataset, not current market evidence.
