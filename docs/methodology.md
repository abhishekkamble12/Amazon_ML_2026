# Methodology

## Overview
This document will describe the technical methodology for the Business Entity Resolution ML pipeline.

### Stages
1. **Data Ingestion & Preprocessing**: Cleaning, normalization, and standardization of entity attributes (name, address, city, state, zip, phone, etc.).
2. **Blocking / Candidate Generation**: Reduction of pairwise comparisons ($O(N^2)$) using multi-index blocking and candidate generation strategies.
3. **Feature Engineering**: Computation of string similarity metrics, token overlap, phonetic encodings, and domain-specific distance metrics.
4. **Classification & Modeling**: Training binary classifiers / ranking models to predict entity match probability.
5. **Threshold Tuning & Post-Processing**: Optimal decision boundary determination, transitive closure / clustering, and final pair resolution.
