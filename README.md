# Employment and Mobility Patterns in Counties of England & Wales (2011) with Age Comparison to 2021

## Overview

This project investigates socio-economic and mobility patterns across county-level local authorities in England and Wales using UK Census data. The analysis combines demographic, economic, transportation, and vehicle ownership indicators from the 2011 Census with age structure data from the 2021 Census to explore regional disparities and demographic changes over a decade.

The project applies dimensionality reduction, clustering, Bayesian analysis, and interactive visual analytics to identify distinct socio-economic profiles across 174 county-level local authorities.

## Objectives

The main objectives of this study are:

- Examine regional differences in employment, mobility, car ownership, and age structure.
- Compare age demographics between 2011 and 2021.
- Identify underlying socio-economic patterns using dimensionality reduction techniques.
- Group counties into meaningful socio-economic clusters.
- Explore probabilistic relationships between socio-economic variables using Bayesian methods.
- Present findings through an interactive Tableau dashboard.

---

## Dataset

The analysis uses UK Census data for England and Wales at the county-level local authority scale.

### 2011 Census Datasets

- Age Structure
- Economic Activity
- Distance Travelled to Work
- Car Ownership

### 2021 Census Dataset

- Age Structure (used for decade-long demographic comparison)

### Coverage

- 174 County-Level Local Authorities
- England and Wales

## Data Preparation

The original census datasets contained highly granular variables. To improve interpretability and support comparative analysis, variables were aggregated into broader socio-economic indicators.

Examples include:

| Original Variables | Aggregated Feature |
|-------------------|-------------------|
| Individual age bands | Youth, Working-Age, Retired Population |
| Detailed commute distances | Short, Medium, Long Commutes |
| Vehicle ownership categories | Car Ownership Indicators |
| Economic activity classes | Employment Activity Indicators |

Both absolute counts and proportional measures were analysed to account for differences in population size across counties.

---

## Methodology

### 1. Data Transformation

- Data cleaning and preprocessing
- Feature aggregation
- Standardisation and normalization

### 2. Dimensionality Reduction

Three techniques were explored:

- Principal Component Analysis (PCA)
- t-Distributed Stochastic Neighbor Embedding (t-SNE)
- Uniform Manifold Approximation and Projection (UMAP)

UMAP was selected as the primary technique due to its ability to preserve local and global structure while producing meaningful cluster separation.

### 3. Clustering Analysis

UMAP embeddings were used to identify socio-economic groupings across counties.

Four distinct clusters emerged from the analysis.

### 4. Bayesian Analysis

Posterior distributions were used to investigate probabilistic relationships between:

- Economic activity
- Commuting behaviour
- Car ownership
- Demographic structure

This approach provided insights into the strength and uncertainty of relationships among variables.

### 5. Visual Analytics

Interactive dashboards were developed using:

- Tableau

The dashboard enables:

- Regional comparisons
- Cluster exploration
- Geographic analysis
- Temporal age comparisons
- Interactive filtering and drill-down

## Identified Clusters

### Cluster 1: Ageing, Long Commute Workforce

**Characteristics:**

- Older population structure
- Longer commuting distances
- Lower local employment accessibility

### Cluster 2: Locally Employed, Mixed Mobility Communities

**Characteristics:**

- Strong local employment patterns
- Diverse mobility behaviour
- Balanced socio-economic indicators

### Cluster 3: High Employment, High Mobility, Multi-Car Areas

**Characteristics:**

- High economic activity
- Greater mobility
- Higher rates of multi-car ownership

### Cluster 4: Low Mobility, Car-Limited Areas

**Characteristics:**

- Lower vehicle ownership
- Reduced mobility
- Potentially constrained access to employment opportunities

---

## Key Findings

### Employment and Mobility

- Regions with higher economic activity generally exhibit greater mobility.
- Multi-car ownership is associated with increased commuting flexibility.
- Proximity to workplaces appears to be a stronger driver of economic activity than vehicle ownership alone.

### Demographic Change

- Comparison between 2011 and 2021 indicates a gradual ageing of the population.
- Several regions experienced significant shifts toward older age structures over the decade.

### Spatial Patterns

- Socio-economic clusters are geographically concentrated rather than randomly distributed.
- Central England contains many high-employment, high-mobility areas.
- Parts of Wales, Northern England, and South-West England display ageing populations and longer commuting patterns.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- UMAP
- PCA
- Bayesian Analysis
- Tableau
