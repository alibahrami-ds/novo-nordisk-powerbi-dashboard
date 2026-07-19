# Novo Nordisk – Key Performance Dashboard (Power BI)

An interactive Power BI dashboard tracking Novo Nordisk's key financial and
operational metrics from 2015 to 2024.

## Objective

While the companion SQL/Python project (Novo-Nordisk-Revenue-Analysis) looks
at revenue trends in detail, this dashboard takes a broader operational view:
revenue, workforce growth, profitability, and R&D investment side by side, to
see how they move together over time.

## Data Source

All figures are taken from Novo Nordisk's official public disclosures:
- Annual Reports / 20-F filings (SEC EDGAR / investor relations site)
- Historical revenue and employee data cross-checked against MacroTrends

Operating margin and R&D cost figures are only available for 2022-2024 in
this dataset; earlier years are left blank rather than estimated.

## Dashboard Contents

**Page 1 – Overview:**
- **KPI cards** (latest year, 2024): total revenue, year-end employees,
  operating margin, R&D costs
- **Revenue trend** (2015-2024): column chart
- **Employee growth** (2015-2024): column chart

**Page 2 – Trends & Forecast:**
- **Operating margin trend** (2022-2024): line chart
- **Revenue YoY growth rate**: line chart, calculated with a DAX measure
- **Revenue forecast**: a What-if parameter lets the viewer adjust an
  assumed growth rate and see a projected 2027 revenue figure update
  live, plus a line chart comparing actual revenue against the forecast

## Key Findings

- Revenue grew roughly 162% from 2015 to 2024, while headcount grew about
  89% over the same period — revenue grew nearly twice as fast as the
  workforce, pointing to a marked increase in productivity.
- Operating margin improved from 42.3% (2022) to 44.2% (2023-2024),
  showing that growth has come with better profitability, not just higher
  sales volume.
- R&D spending roughly doubled between 2022 and 2024, in line with the
  company's expanding product pipeline.

## Tools

- Power BI Desktop
- DAX (for the year-over-year growth measure and the revenue forecast)

## Files

- `Novo_Nordisk_PowerBI_Dashboard.pbix` – the dashboard file (open with Power BI Desktop)
- `novo_nordisk_kpis.csv` – source data
