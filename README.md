# Spillover Effects of Financial Inclusion on Consumption Patterns in Rural Peruvian Families

**Alejandro Armas Braithwaite and Emanuel Paredes Salazar**
Research paper (master's thesis), Master in Economics, Pacífico Business School (Lima, Peru), 2019
Advisor: Prof. Francisco Galarza Arellano

📄 Paper: [English version](TI_Armas_Paredes_EN.pdf) · [Versión en español](TI_Armas_Paredes.pdf)

---

## Research question

At the end of 2017, 64.9% of Peru's districts had no physical presence of the financial system (no bank branch, ATM, or banking agent). This project asks whether rural households living in these unserved districts still benefit **indirectly** from being physically close to a district that does have financial services, and whether that proximity changes how they spend.

We study two outcomes related to household welfare:

1. **The share of spending devoted to durable goods** (long-term assets), and
2. **Total household spending.**

## Data

| Source | What it provides | Period |
|---|---|---|
| ENAHO (Encuesta Nacional de Hogares), INEI | Household expenditure composition and household-head characteristics (annual cross-sections) | 2010–2017 |
| SBS (Superintendencia de Banca, Seguros y AFP) | District-level financial access (banks, municipal savings banks, banking agents) and use (credits, deposits) | 2010–2017 |

Indirect access is measured as the distance from each unserved district to the **nearest district with at least one banking agent** (*cajero corresponsal*, the most widespread type of financial access point in Peru), grouped into three bands: up to 20 km, 20 to 50 km, and more than 50 km (reference group).

Both sources are publicly available. Raw data are not stored in this repository; see [Data access](#data-access) below.

## Methodology

ENAHO's panel modules do not include disaggregated expenditure, so we use the annual cross-sections and build **pseudo-panels** (Verbeek 2008). Households are grouped into cohorts defined by time-invariant characteristics: locality stratum, mother tongue, and the household head's birth-year range. We then estimate **within (fixed-effects) models** on cohort means.

Because financial institutions choose where to expand based on market conditions, access and use may be correlated with unobserved factors that also affect spending. To address this, we **instrument access and use variables with their one-period lags**, following Berhane and Gardebroek (2011).

Controls include the household head's sex, employment status, marital status, education level, and use of financial services. Robustness checks include an interaction between bank and municipal-savings-bank credit, disaggregated deposits, squared access terms, a market-concentration (HHI) specification, and an aggregated model.

## Main findings

- **Durable goods:** Households in unserved districts located within 50 km of a district with a banking agent devote a larger share of spending to durable goods than households more than 50 km away. The effect is significant at the 1% level across all specifications.
- **The effect grows with proximity:** The coefficient for households within 20 km (0.0033 to 0.0041) is nearly double that for households 20 to 50 km away (0.0018 to 0.0025).
- **Total spending:** The effect on total spending is negative and significant at the 1% level for both distance bands, but smaller in magnitude for households closer to financial services.
- **Interpretation:** Even without direct access to or use of the financial system, proximity to districts with financial presence robustly changes consumption patterns, shifting spending toward long-term assets.

See the paper for full results, discussion, and policy recommendations.

## Repository structure

```
├── README.md
├── TI_Armas_Paredes_EN.pdf   # English version
├── TI_Armas_Paredes.pdf      # Original Spanish version
├── code/                     # Replication code (to be added)
└── output/                   # Tables and figures (to be added)
```

## Replication

Replication code will be added to `code/`. This section will describe the execution order, software requirements, and how each script maps to the tables in the paper.

## Data access

- **ENAHO:** INEI microdata portal (Peru's National Institute of Statistics and Informatics).
- **SBS:** Public statistics on financial access points and credit/deposit indicators by district.

## Citation

Armas Braithwaite, A., and Paredes Salazar, E. (2019). *Spillover Effects of Financial Inclusion on Consumption Patterns in Rural Peruvian Families* [Research paper, Master in Economics, Pacífico Business School].

## Contact

Alejandro Armas Braithwaite · alarmasb@uchicago.edu · [alejandroinfo.github.io](https://alejandroinfo.github.io)
