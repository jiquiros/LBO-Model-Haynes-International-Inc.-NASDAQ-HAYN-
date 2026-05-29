# LBO Model — Haynes International, Inc. (NASDAQ: HAYN)

**Project:** Hypothetical PE LBO analysis using real public data  
**Unique angle:** Acerinox acquired Haynes at $970M in January 2025 — this model uses the same entry price structured as a PE buyout, then answers: *would a financial sponsor have generated 20%+ IRR at that price?*

---

## What this is

A full leveraged buyout model built on real public financials (Haynes International 10-K FY2023, SEC 8-K filings, and the Acerinox deal announcement). All data is sourced from publicly available documents — no proprietary or non-public information.

> Haynes International manufactures high-performance nickel and cobalt alloys for aerospace (~54% of revenue), industrial gas turbines, and chemical processing. It was acquired by Acerinox S.A. in January 2025 for $970M (12.3x EBITDA FY2023).

---

## Files in this repository

| File | Description |
|------|-------------|
| `Haynes_International_LBO_Model.xlsx` | Full 8-tab LBO model |
| `README.md` | This file |

---

## Excel model — 8 tabs

| Tab | Content |
|-----|---------|
| **Assumptions** | All inputs in blue: revenue growth, EBITDA margins, capex, debt terms, entry/exit multiples. Every projection cell links here. |
| **Income Statement** | FY2021–2023 actuals (sourced), FY2024E–2028E projections. Revenue → EBITDA → EBIT → Net income with interest linked to Debt Schedule. |
| **Debt Schedule** | Term Loan B ($314M @ 8.5%) and Senior Notes ($118M @ 9.5%). Annual amortization, interest, covenant tests (Net Leverage and Interest Coverage). |
| **Free Cash Flow** | EBITDA → taxes → capex → NWC change → levered FCF. Unlevered and levered builds separated. |
| **Returns Analysis** | IRR and MOIC across 3 exit scenarios (10x / 12x / 14x EBITDA at Year 5). Value creation bridge: EBITDA growth + multiple expansion + debt paydown. |
| **Sensitivity** | Two 5×5 tables with color scale: (1) IRR by entry vs. exit multiple; (2) MOIC by revenue CAGR vs. EBITDA margin. |
| **Valuation Bridge** | Decomposition of equity value entry → exit with explicit attribution to each value creation lever. |
| **vs. Acerinox Deal** | Direct comparison: PE LBO returns at $970M entry vs. Acerinox's all-cash strategic acquisition. Includes analytical conclusion on strategic vs. financial buyer pricing. |

---

## Deal snapshot — real transaction

| Parameter | Value | Source |
|-----------|-------|--------|
| Acquiror | Acerinox S.A. | BusinessWire, Feb 5 2024 |
| Price per share | $61.00 (all-cash) | Definitive agreement |
| Equity value | $798M | 13.08M shares × $61 |
| Enterprise value | $970M | Equity + $172M net debt/adj. |
| EV / EBITDA FY2023 | 12.3x | Deal announcement |
| Premium to 6-mo VWAP | ~22% | Calculated |
| Close | January 2025 | Acerinox press release |

---

## Hypothetical LBO structure

| Parameter | Value |
|-----------|-------|
| Entry EV | $970M (same as Acerinox) |
| Term Loan B | $314M (~4.0x EBITDA) @ 8.5% |
| Senior Notes | $118M (~1.5x EBITDA) @ 9.5% |
| Total leverage | 5.5x EBITDA at entry |
| Sponsor equity | ~$538M |
| Hold period | 5 years (exit FY2028E) |

---

## Key findings

**Base case (12x exit, 7% rev CAGR, 14.5% EBITDA margin):**  
IRR ~18–19% — below the 20%+ PE target. Deal is marginal for a financial sponsor at $970M.

**Upside case (14x exit, 9% CAGR):**  
IRR ~24% — here the deal works for PE. Requires both multiple expansion and above-base revenue growth.

**Main conclusion:** Acerinox, as a strategic buyer with a ~8–10% hurdle rate, could justify $970M where a PE fund could not at base case. A financial sponsor would likely have required ~$820–850M to generate 20%+ IRR comfortably. The model quantifies exactly why strategic and financial buyers reach different valuations for the same asset.

---

## Modeling assumptions & limitations

- Revenue projections (5–8% growth) are forward-looking estimates based on Haynes's disclosed backlog ($405M as of Q3 2024) and aerospace market tailwinds; not management guidance
- EBITDA margin expansion (13% → 16.5%) reflects operational leverage assumptions — actual margins depend heavily on nickel/cobalt input costs, which are volatile
- Debt terms (rates, amortization) are modeled based on 2024 leveraged loan market conditions — actual terms would differ
- Tax rate (25%) is an effective rate approximation; actual deferred tax treatment in an LBO context would require detailed tax analysis
- Cash sweep circularity is simplified (no iterative solver) — in a real model this would use Excel's circular reference setting

---

## Skills demonstrated

- LBO model architecture (8-tab, fully linked)
- Debt structuring (TLB + HY Notes, covenant modeling)
- Free cash flow analysis (unlevered and levered)
- IRR / MOIC returns analysis with sensitivity
- Value creation waterfall (EBITDA growth / multiple expansion / debt paydown)
- Real deal benchmarking (strategic vs. financial buyer pricing logic)
- Financial data sourcing from SEC EDGAR (10-K, 8-K)

---

## Data sources

- Haynes International 10-K FY2023 (SEC EDGAR)
- Haynes International 8-K filings Q3 2024 (SEC EDGAR)
- Acerinox press release — February 5, 2024 (BusinessWire)
- Acerinox press release — transaction close, January 2025

---

## Other projects in this portfolio

| Project | Description |
|---------|-------------|
| [M&A Model — CloudCore / DataStream](https://github.com/jiquiros/ma-financial-model) | EPS accretion/dilution model for SaaS acquisition. Fictional case calibrated to real market benchmarks. |
| Valuation — Full DCF + Comps + Precedents | *Coming soon* |
| IPO Analysis | *Coming soon* |

---

*For questions or feedback, connect on [LinkedIn](www.linkedin.com/in/jose-isaac-quiros-b348a7217)*

*All analysis is for educational and portfolio purposes only. Not investment advice. All projections are the author's own estimates based on publicly available data.*
