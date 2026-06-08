# Kaya decomposition using multiple data sources

This repository contains an exploratory analysis of fossil fuel CO₂ emissions using the Kaya identity framework.

## Objective

The objective is to decompose changes in fossil CO₂ emissions into four driving factors:

* Population
* GDP per capita
* Energy intensity of the economy
* Carbon intensity of the energy system

## Methodology

The analysis is based on the Kaya identity:

CO₂ = Population × (GDP / Population) × (Energy / GDP) × (CO₂ / Energy)

Two complementary approaches are used:

### 1. Annual logarithmic Kaya decomposition

Annual changes in emissions are decomposed using logarithmic growth rates:

Δln(CO₂) = Δln(P) + Δln(GDP/P) + Δln(E/GDP) + Δln(CO₂/E)

This allows annual emission changes to be attributed to individual Kaya factors.

### 2. LMDI decomposition

For selected periods, the Logarithmic Mean Divisia Index (LMDI) method can be used to decompose cumulative changes in emissions between two years.

## Data sources

### World Bank

* Population (SP.POP.TOTL)
* GDP, constant 2015 US$ (NY.GDP.MKTP.KD)

### Energy Institute Statistical Review of World Energy

* Total Energy Supply (TES)
* Fossil fuel combustion CO₂ emissions

## Countries analysed

Completed:

* China (1990–2024)
* United States (1990–2024)
* United Kingdom (1990–2024)
* Germany (1990–2024)

Planned:

* Czech Republic
* Japan
* India
* European Union

## Repository structure

```text
README.md
Kaya_ruzna_data.ipynb

data/
figures/
sources/
```

## Outputs

For each country the repository contains:

* processed dataset
* annual Kaya decomposition dataset
* decomposition figure

## Status

Work in progress.
