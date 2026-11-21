# TraceWise — Dataset Quality Auditor

A lightweight, browser-based CSV quality auditor. It profiles columns, counts missing values, detects exact duplicate rows, flags potential numeric outliers with the IQR rule, calculates an explainable heuristic score, and exports a JSON report.

## Run
No Python, Node.js, package installation, API key, or backend is needed.

1. Extract this folder.
2. Double-click `index.html` or right-click → Open with Chrome / Edge.
3. Click **Load sample dataset** or choose your own CSV.
4. Explore findings and click **Export report**.

Optional local server:
```bash
python -m http.server 5500
```
Open `http://localhost:5500`.

## Notes
All processing happens in the browser; files are not uploaded. The demo supports CSV files up to 10 MB and 100,000 rows. Outliers are potential anomalies, not confirmed errors. The quality score is a heuristic, not a universal data-quality standard. Date-like columns are profiled as text.
