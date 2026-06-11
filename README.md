# Afficionado Coffee Roasters — Sales & Store Insights Dashboard

A Streamlit-based interactive dashboard and analysis package for Afficionado Coffee Roasters. The project provides temporal sales analysis, product and category revenue breakdowns, hourly demand heatmaps, and store-level comparisons to support operational decisions such as staffing, inventory and promotions.

## Table of Contents
- [Introduction](#introduction)
- [Dataset / Inputs](#dataset--inputs)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Analysis & Features](#analysis--features)
- [Results & Insights](#results--insights)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

This repository contains the code, assets, and documentation for an interactive sales analytics dashboard built with Streamlit. The dashboard helps visualize overall sales trends, day-of-week performance, hourly demand patterns, and store/product comparisons.

## Dataset / Inputs

- Transaction and product exports from the point-of-sale system. A SQL extract script is included at `SQL/Afficionado Coffee Roasters.sql`.
- Project-level data files (CSV/exports) should be placed in the `Data/` folder. If you plan to reproduce the analysis, provide the transaction CSV(s) with columns for timestamp, store_location, product identifiers, quantity, and revenue.

If you want me to ingest specific CSV files and populate the Results section with numeric tables, upload them to the `Data/` folder or grant access.

## Tech Stack

- Streamlit — interactive web UI
- Python — data processing and scripting
- pandas — data manipulation
- plotly / seaborn / matplotlib — visualizations
- SQL — data extraction and preprocessing

## Installation

Recommended (Windows) example:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r Streamlit-App\ requirements.txt
```

If you don't have a `requirements.txt`, install the core libraries:

```powershell
pip install streamlit pandas plotly seaborn
```

## Usage

Run the Streamlit application from the `Streamlit-App Dashboard` folder (adjust filename if different):

```powershell
cd "Streamlit-App Dashboard"
streamlit run app.py
```

Live deployment (view-only):

https://coffeeroastersstreamlight-atu2r3dukjq7dmjyvmyaab.streamlit.app/

## Analysis & Features

- Overall sales trend dashboard — revenue and quantity trends over time
- Day-of-week performance charts — compare weekdays for demand planning
- Hourly demand heatmaps — visualize recurring daily peaks and troughs
- Location comparison panels — side-by-side revenue and product mix by store
- Interactive controls: store location filter, day-of-week selector, hour-range slider, revenue vs quantity toggle

Business questions addressed:
- When are the busiest hours by store and product?
- Which products contribute the most to revenue?
- How does performance vary between store locations?

## Results & Insights

Key takeaways (derived from dashboard visuals):
- Peak demand typically concentrates in morning hours — useful for scheduling staff.
- A small set of product details contribute a large share of revenue — consider targeted inventory and promotions.
- Store-level comparisons reveal differences in revenue mix that warrant localized merchandising.

For numeric tables and specific aggregates, place raw CSVs in `Data/` and I can compute and add detailed result tables.

## Project Structure

- `Dashboards/` — exported dashboard images and assets
- `Data/` — raw and processed data files (CSV)
- `SQL/` — SQL extraction and transformation scripts
- `Streamlit-App Dashboard/` — Streamlit app source, `app.py`, and run instructions
- `Presentation/` — slide decks and presentation assets
- `Report/` — research paper and reports (includes `Research_Paper.md`)

## Contributing

Contributions are welcome. Typical workflow:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Make changes and add tests where applicable
4. Submit a pull request with a clear description of changes

Please open issues for bug reports or feature requests.

## License

This project includes a `LICENSE` file at the repository root. Please refer to it for the project's license terms.

## Contact

- Name: Nikita Gautam
- Email: nikitagautam647@gmail.com
- Streamlit dashboard (deployed): https://coffeeroastersstreamlight-atu2r3dukjq7dmjyvmyaab.streamlit.app/


