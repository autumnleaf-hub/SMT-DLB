# Input and Paper Result Data

This directory contains the experiment input data and the paper result data used by the dynamic DDLB experiments.

## Directory Layout

- `configs/`: experiment configuration, algorithm list, seed list, and matrix settings.
- `data/instances/`: 36 dynamic DDLB instances. Each instance contains static job-resource information and 10 dynamic environment snapshots.
- `data/offline_archives/`: historical elite solution archives for each instance and environment.
- `data/reference_fronts/`: reference Pareto fronts for metric calculation.
- `data/memory_bank_init/`: initial memory bank used by transfer-based algorithms.
- `outputs/paper_results/`: result tables and figure source data matching the paper experiment section.

## Input Matrix

- Instances: 36
- Dynamic environments per instance: 10
- Seeds: 8
- Algorithms: SMT-DLB, CI-DMOEA, DG-DMOEA, SET, KTS-DMOEA, CBT

## Paper Result Files

- `outputs/paper_results/tables/migd.csv`: MIGD table values.
- `outputs/paper_results/tables/mhv.csv`: MHV table values.
- `outputs/paper_results/tables/art.csv`: ART table values.
- `outputs/paper_results/tables/nigd.csv`: NIGD table values.
- `outputs/paper_results/tables/ablation.csv`: ablation table values.
- `outputs/paper_results/figures/fig_convergence_data.csv`: convergence curve source data.
- `outputs/paper_results/figures/fig_tradeoff_data.csv`: MHV-ART tradeoff figure source data.
- `outputs/paper_results/figures/fig_nigd_data.csv`: NIGD figure source data.
- `outputs/paper_results/environment_metrics.csv`: full instance-seed-environment metric table.

## Data Meaning

- `migd`: mean inverted generational distance; lower is better.
- `mhv`: mean hypervolume; higher is better.
- `art`: average response time; lower is better.
- `nigd`: normalized IGD improvement ratio.

