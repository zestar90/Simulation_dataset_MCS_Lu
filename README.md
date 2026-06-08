# Simulation Dataset for District-Scale Seismic Risk Assessment of Tehran

## Description

This repository contains the simulation-generated dataset used in the study:

**"A Scenario-Based Framework for District-Scale Seismic Risk Assessment: Application to Tehran, Iran"**

The dataset was developed to support machine-learning-based prediction of post-earthquake building damage and district-scale seismic risk assessment under alternative earthquake scenarios in Tehran, Iran.

## Dataset Overview

The dataset was generated using nonlinear structural analyses of representative building typologies subjected to earthquake ground motions. The resulting structural response, seismic demand parameters, and building characteristics were compiled into a database for machine-learning model development and evaluation.

Each row represents a simulated building-earthquake scenario.

## Main Variables

The dataset includes variables describing:

* Building structural system
* Building height class
* Construction age/code level
* Seismic demand parameters
* Ground-motion intensity measures
* Structural response indicators
* Damage state classification

## Target Variable

The machine-learning models were developed to predict post-earthquake damage states corresponding to rapid safety assessment categories:

* **Green** – Safe for occupancy
* **Yellow** – Restricted use / requires further inspection
* **Red** – Unsafe / restricted access

## File Format

The dataset is provided in Apache Parquet format:

* `Simulation_dataset_MCS_Lu.parquet`

The dataset can be loaded in Python using:

```python
import pandas as pd

df = pd.read_parquet("Simulation_dataset_MCS_Lu.parquet")
```

## Related Publication

Monir Vaghefi, Z., Asgarian, B.

*A Scenario-Based Framework for District-Scale Seismic Risk Assessment: Application to Tehran, Iran.*

Submitted to the Journal of Earthquake Engineering.

## Citation

If you use this dataset, please cite the associated publication when available.

## License

This repository is made available for academic and research purposes.
