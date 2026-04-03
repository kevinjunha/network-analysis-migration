# Social Network Analysis of Global Remittance Flows & Syrian Transnational Migration

**Kevin Jun Ha**

## Overview

This project applies social network analysis (SNA) to global bilateral remittance data to examine the transnational network of the Syrian Arab Republic. Using KNOMAD's bilateral remittance matrices as a foundation, I constructed a country-level network where nodes represent countries and edges represent remittance relationships — treating any financial flow (sent or received) as evidence of maintained transnational ties.

The project spans the full data pipeline: from raw KNOMAD matrices → data transformation → network construction → centrality analysis → visualization.

## Research Question

How is Syria positioned within the global remittance network, and what does this reveal about its transnational migration relationships? Following Portes, Guarnizo, and Landolt's (1999) concept of migrants "living dual lives," remittance flows — regardless of direction — serve as observable evidence of sustained cross-border connection.

## Key Findings

- **207 nodes** (countries) and **~4,337 edges** in the network
- **Average degree of ~41.9** — each country maintains remittance ties with roughly 42 others on average
- **Network diameter of 3** — the maximum distance between any two countries in the remittance flow network is just 3 steps
- Top nodes by centrality (betweenness, closeness, degree, eigenvector): United States, France, United Kingdom, Canada, Australia
- Syria has **direct (1-step) remittance connections** to Iraq and West Bank & Gaza, and is reachable from all top centrality countries in 1–2 steps

## Methods & Tools

- **Language:** Python
- **Libraries:** NetworkX, pandas, matplotlib, plotly, NumPy
- **Centrality measures:** Degree, Betweenness, Closeness, Eigenvector
- **Data source:** KNOMAD Bilateral Remittance Matrices (transformed to edgelist/nodelist format)

## Repository Structure

├── Remittances_SNA_KevinJunHa.ipynb   # Main analysis notebook
├── data/
│   ├── raw/                            # Original KNOMAD bilateral remittance matrices
│   └── processed/
│       ├── remittance_edgelist_noweight2.csv
│       └── remittance_nodelistv3.csv
└── images/                             # Network visualizations

## Visualizations

Five network graphs were produced, each sizing and coloring nodes by a different centrality measure: degree, betweenness, closeness, and eigenvector centrality, plus a degree distribution histogram.

## Skills Demonstrated

`Python` · `NetworkX` · `Social Network Analysis` · `pandas` · `Data Wrangling` · `matplotlib` · `Quantitative Research` · `Migration Studies`

## Background

This project was completed as part of graduate-level coursework in computational social science, with a substantive focus on transnational migration theory.
