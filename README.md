# Causality from Molecular Dynamics Simulations
Correlation is not causation. Molecular dynamics (MD) simulations provide a detailed description of the structural fluctuations and correlated motions that occur within biomolecular systems. However, correlation alone does not establish whether fluctuations in one region precede or contribute to changes in another.

Here, we present a reproducible approach based on Granger causality to identify directional, time-dependent relationships from MD trajectories and investigate how dynamical changes propagate across biomolecular systems.

Granger causality is a time-series approach that asks a simple question: Does the past behavior of feature X help predict the future behavior of feature Y? If including the history of X significantly improves the prediction of Y beyond what can be predicted from Y alone, X is said to Granger-cause Y.

This repository provides a practical workflow for applying this concept to molecular simulations. The notebook:
extracts structural features from MD trajectories; constructs time series describing protein and DNA dynamics; applies Granger causality analysis to identify directional relationships; evaluates statistical significance; and combines results across independent MD replicas to obtain ensemble-level statistics.

The workflow was developed to investigate how changes in protein structural dynamics can precede changes in DNA structural features, but it can be readily adapted to other biomolecular systems and user-defined structural descriptors.

This notebook performs Granger causality analysis on MD simulations to investigate directional relationships between protein structural dynamics and DNA structural features. The analysis is performed across multiple simulation replicas and the results are aggregated to obtain ensemble statistics.

The workflow extracts structural features from MD trajectories, applies time-series modeling, and identifies statistically significant causal relationships between defined protein regions and DNA structural properties.

Citation: If you use this code
PAPER/DOI : https://doi.org/10.1101/2025.06.17.659969

<p align="center">
  <img src="Figure 3.tif" width="900">
</p>


License: MIT License
