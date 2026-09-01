# 🍽️ Restaurant Analytics & Insights

> End-to-end data analytics project that transforms restaurant data into actionable business insights using Python, SQL, Jupyter and Power BI.

[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)]()
[![Python](https://img.shields.io/badge/Python-Analysis-3776AB?style=for-the-badge&logo=python&logoColor=white)]()
[![SQL](https://img.shields.io/badge/SQL-Data%20Analysis-4479A1?style=for-the-badge&logo=mysql&logoColor=white)]()
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)]()
[![License](https://img.shields.io/badge/License-MIT-blue.svg)]()

---

## Quickstart

1. Clone the repo

   ```bash
   git clone https://github.com/Ritti902/Restaurant-analytics-insights.git
   cd Restaurant-analytics-insights
   ```

2. Create environment and install dependencies

   - With pip:

     ```bash
     python -m venv .venv
     source .venv/bin/activate   # Windows: .venv\Scripts\activate
     pip install -r requirements.txt
     ```

   - Or with conda:

     ```bash
     conda env create -f environment.yml
     conda activate restaurant-analytics
     ```

3. Run notebooks

   ```bash
   jupyter lab
   # or
   jupyter notebook
   ```

   Open notebooks in /notebooks:
   - 01_Data_Cleaning.ipynb
   - 02_Exploratory_Analysis.ipynb
   - 03_Restaurant_Performance.ipynb
   - 04_Customer_Insights.ipynb

4. Open report
   - Open `reports/Restaurant_Business_Intelligence.pbix` in Power BI Desktop to explore the interactive dashboard.

---

## Files & Structure

```text
Restaurant-Analytics-Insights/
├── data/
│   ├── raw_dataset.csv
│   ├── restaurant_cleaned.csv
│   └── processed_datasets/
├── notebooks/
│   ├── 01_Data_Cleaning.ipynb
│   ├── 02_Exploratory_Analysis.ipynb
│   ├── 03_Restaurant_Performance.ipynb
│   └── 04_Customer_Insights.ipynb
├── reports/
│   └── Restaurant_Business_Intelligence.pbix
├── screenshots/
│   ├── dashboard_overview.png
│   ├── customer_performance.png
│   └── market_insights.png
├── requirements.txt
├── environment.yml
└── README.md
```

---

## Data

- `data/raw_dataset.csv` — original dataset (add source and license if not public)
- `data/restaurant_cleaned.csv` — cleaned dataset used in analysis
- `data/processed_datasets/` — intermediate aggregated datasets used by notebooks

Data dictionary (add or adjust types as needed):
- `restaurant_id` (string/int): unique identifier
- `name` (string): restaurant name
- `city` (string): city name
- `average_cost_for_two` (numeric): average cost for two
- `cuisines` (string): cuisine types (comma-separated)
- `aggregate_rating` (numeric): rating score
- `votes` (int): number of votes/reviews
- `online_delivery` (0/1): online delivery availability
- `has_table_booking` (0/1): table booking availability
- `price_range` (1-4): price category
- (Add any additional columns and types)

Privacy notes
- If using real data, redact or anonymize any personal or sensitive fields and state any usage restrictions.

---

## How to reproduce / scripts

- `01_Data_Cleaning.ipynb` — cleans `raw_dataset.csv` and generates `restaurant_cleaned.csv`
- `02_Exploratory_Analysis.ipynb` — EDA charts & pivot tables
- `03_Restaurant_Performance.ipynb` — KPIs and performance metrics
- `04_Customer_Insights.ipynb` — customer behavior analysis and correlations

Helpful commands

- Export notebook to HTML:

  ```bash
  jupyter nbconvert --to html notebooks/02_Exploratory_Analysis.ipynb
  ```

- Recreate cleaned CSV (if you provide a script):

  ```bash
  python scripts/clean_data.py --input data/raw_dataset.csv --output data/restaurant_cleaned.csv
  ```

---

## Key findings (replace with your actual results)
- Top cuisines by number of restaurants: (e.g., North Indian, Chinese, Fast Food)
- Cities with highest average cost for two: (e.g., City A, City B)
- Positive correlation between votes and aggregate_rating (more engagement → better ratings)
- Price range varies significantly by cuisine and city
- Online delivery and table booking adoption: X% and Y% of restaurants respectively

Replace the bullets above with concrete numbers and short charts from your notebooks for an executive summary.

---

## Visuals / Demo

![Dashboard overview](screenshots/dashboard_overview.png)
![Customer performance](screenshots/customer_performance.png)

If you host a live demo or publish the report, add the link here.

---

## Requirements

Include a `requirements.txt` or `environment.yml` (example packages and suggested versions):

```
pandas
numpy
matplotlib
seaborn
jupyterlab
openpyxl
sqlalchemy
ipykernel
```

Pin versions when possible. If you would like, I can generate a `requirements.txt` with pinned versions from your notebooks.

---

## Contributing

Contributions welcome!
- Open an issue first to discuss major changes
- Fork the repo and send a PR
- Include tests or outputs for new analyses

Consider adding `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md` if you expect external collaborators.

---

## License

This project is licensed under the MIT License — see `LICENSE` file for details. If you prefer a different license (Apache-2.0, GPL-3.0), update accordingly.

---

## Contact

Maintainer: `Ritti902`

---

## Next steps I can do for you
- Create `requirements.txt` or `environment.yml` with pinned versions based on your notebooks
- Add a `DATA_DICTIONARY.md` with full column descriptions
- Add `CONTRIBUTING.md` and `LICENSE` files

If you'd like me to add any of the above files, tell me which and I'll add them to the repository.
