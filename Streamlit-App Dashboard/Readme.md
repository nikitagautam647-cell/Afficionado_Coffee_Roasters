# Afficionado Coffee Roasters — Streamlit Dashboard

This Streamlit web application provides interactive analysis of Afficano Coffee Roasters' sales data. The dashboard implements the requested features and includes instructions for installation and usage below.

## Summary
- Overall sales trend dashboard
- Day-of-week performance charts
- Hourly demand heatmaps
- Location comparison panels

## Core Modules
- Overall sales trend dashboard — Displays total revenue and quantity trends over time.
- Day-of-week performance charts — Compare performance by weekday (counts, averages, totals).
- Hourly demand heatmaps — Hour-by-hour demand heatmap with intensity coloring.
- Location comparison panels — Side-by-side comparisons for different store locations.

## User Controls
- Store location filter — Select one or more stores to include.
- Day-of-week selector — Filter data by a specific weekday.
- Hour-range slider — Select a range of hours to focus analysis.
- Revenue vs Quantity toggle — Switch charts between revenue and quantity metrics.

## Installation
Example setup on Windows:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

If you don't have a `requirements.txt`, install at least:

```powershell
pip install streamlit pandas plotly seaborn
```

## Run
From the project folder (Streamlit-App Dashboard) run:

```powershell
streamlit run app.py
```

Replace `app.py` with the actual main script filename if different.

## Usage
- Use the controls at the top of the page to select `Store location`, `Day-of-week`, and `Hour-range`.
- Toggle `Revenue vs Quantity` to change chart metrics.
- Hover on heatmap cells to see hour-level values and tooltips.

## Files
- `app_link.txt` — If present, contains a quick link or deployment host information.

## Notes & Tips
- For large datasets, apply caching or sampling in preprocessing steps to improve performance.
- If the data source is SQL, keep connection credentials in environment variables and not in code.

## Contact
If you'd like further details added to this README or an example `requirements.txt` and `app.py`, tell me which language (English/Hindi) and I'll add them.

