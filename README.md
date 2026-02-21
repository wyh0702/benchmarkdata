# benchmarkdata

This repository contains benchmark datasets used for systematic evaluation of TCR–pMHC prediction models. The database is organized into three major components:

## 1. Baseline Performance Benchmark

This dataset is designed to evaluate the fundamental predictive performance of models.  
It consists of two major categories:

- **Non-human antigens** (four key pathogens—Cytomegalovirus (CMV), Epstein-Barr virus (EBV), Influenza A (FluA), and Human Immunodeficiency Virus (HIV))
- **Human-derived antigens**

These datasets are used to assess standard classification performance under conventional experimental settings.

## 2. Generalization Benchmark

This dataset is constructed to evaluate model generalization ability to unseen epitopes.

- The **TRAIT database** serves as the primary data source.
- All samples overlapping with any model’s pretraining data were strictly removed.
- The resulting dataset contains epitopes that are completely unseen by the evaluated models.

This benchmark is intended to assess true cross-antigen generalization performance.

## 3. Single-Point Mutation Sensitivity Benchmark

This dataset is designed to evaluate model robustness to directed sequence perturbations.

- The dataset is derived from **LC13-TCR–related experimental data**.
- It focuses on single amino acid mutations to test the model’s ability to detect subtle sequence variations.

This benchmark specifically measures model stability and sensitivity under minimal sequence modifications.
