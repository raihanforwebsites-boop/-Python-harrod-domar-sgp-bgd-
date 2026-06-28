# Harrod-Domar Model: Singapore vs Bangladesh (2004–2023)

An applied analysis of the **Harrod-Domar growth model** using 20 years of World Bank data for Singapore and Bangladesh.

## What This Project Does

The Harrod-Domar model states that:

$$g = \frac{s}{v}$$

Where **g** is GDP growth, **s** is the savings rate, and **v** is the capital-output ratio.

This notebook applies that framework to two contrasting economies — one developed (Singapore) and one developing (Bangladesh) — and visualizes the relationship between savings, capital formation, and growth over 2004–2023.

## Charts Produced

| Chart | Description |
|---|---|
| `sgp_growth.png` | Singapore GDP growth rate with trend line |
| `sgp_cs.png` | Singapore savings vs capital formation |
| `bgd_growth.png` | Bangladesh GDP growth rate with trend line |
| `bgd_cs.png` | Bangladesh savings vs capital formation |
| `comparison_growth.png` | Side-by-side panel comparison |
| `combined_growth.png` | Both countries on one axis |

## Key Findings

- **Singapore** runs a savings surplus (~53% of GDP vs ~25% capital formation), channelling excess savings into sovereign wealth funds. High capital efficiency drives strong growth.
- **Bangladesh** faces a classic Harrod-Domar savings gap — capital formation exceeds domestic savings, bridged by remittances and FDI. Growth is stable at ~6–7%.
- Singapore's growth is higher but more volatile; Bangladesh's is lower but more consistent.

## Data Source

[World Bank Open Data](https://data.worldbank.org)
- `NY.GDP.MKTP.KD.ZG` — GDP growth rate (annual %)
- `NY.GDS.TOTL.ZS` — Gross Domestic Savings (% of GDP)
- `NE.GDI.TOTL.ZS` — Gross Capital Formation (% of GDP)

## How to Run

```bash
pip install pandas matplotlib seaborn numpy openpyxl jupyter
jupyter notebook harrod_domar_analysis.ipynb
```

## Academic Context

Originally submitted as a group assignment for ECO208-3 (Fundamentals of Economic Growth and Development) at Christ (Deemed to Be University), Bengaluru. This version extends the original work with Python-based visualizations and a structured analytical framework.
