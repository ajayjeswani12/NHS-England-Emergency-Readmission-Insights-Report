# NHS Emergency Readmissions Dashboard

A Streamlit dashboard for exploring the NHS England I02040 Compendium Readmissions Dataset.

---

## Files

| File | Purpose |
|---|---|
| `nhs_readmissions_dashboard.py` | Main Streamlit app |
| `requirements.txt` | Python dependencies |

---

## Quick Setup

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Run the app locally

```bash
streamlit run nhs_readmissions_dashboard.py
```

This opens at `http://localhost:8501` in your browser.

### 3. Upload your data

Use the **sidebar file uploader** to load:
```
I02040_Compendium_Readmissions_Dataset__Main__2025.xlsx
```

---

## Deploy to Streamlit Cloud (free)

1. Push both files to a **GitHub repository**
2. Go to [share.streamlit.io](https://share.streamlit.io)
3. Click **New app** → connect your repo → set main file to `nhs_readmissions_dashboard.py`
4. Click **Deploy** — Streamlit handles the rest

> Users upload the Excel file themselves via the sidebar — no data needs to live in the repo.

---

## What's in the Dashboard

| Section | What it shows |
|---|---|
| **National KPIs** | Current rate, decade change, readmission volumes, provider banding counts |
| **Trend + YoY Change** | Line chart for Persons/Male/Female + waterfall of year-on-year pp changes |
| **Geographic Breakdown** | Interactive bar chart — Region, ICB, Deprivation, Treatment Function, or Provider |
| **Deprivation & Equity** | IMD quintile bar chart + trend lines showing the widening deprivation gap |
| **Provider Deep Dive** | Rate distribution histogram, banding donut, ranked best/worst provider tables |
| **Treatment Function** | Specialty rates filtered by minimum readmissions threshold |
| **Raw Data Explorer** | Full filter + CSV download |

---

## Sidebar Controls

- **File uploader** — load the xlsx dataset
- **Year range** — filter all charts to a time window
- **Sex** — toggle Persons / Male / Female across all views
- **Breakdown** — switch the geographic/breakdown section

---

## Data Notes

- Header row is on row 16 of the Data sheet (rows 1–15 are title/metadata)
- Indicator value = emergency readmission rate as a percentage
- Numerator = count of emergency readmissions within 30 days
- Denominator = count of eligible finished admission episodes
- Banding: B = Better than expected, W = Within, A = Alert (above expected)
- 2020/21 is a COVID-19 outlier — denominator fell ~22% while numerator held up

---

## Python Version

Python 3.10+ recommended.
