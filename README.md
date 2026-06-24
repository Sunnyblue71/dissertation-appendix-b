# Dissertation Appendix B: Supplemental Synthetic Benchmark Data

This folder contains the machine-readable data archive supporting the synthetic Stage D evidence reported in Chapters IV and V of:

**Sunday Osiebuni Aghamie (2026), _A DeepSurv-Inspired Inverse Probability of Censoring Weighted Discrete-Time Mixture-of-Experts Survival Framework for Heterogeneous Right-Censored Data_.**

## Evidentiary scope

The files document a finite descriptive benchmark archive. They do not represent a Monte Carlo inferential study and do not provide simulation standard errors, confidence intervals, power, or hypothesis-test quantities.

The verified Stage D archive contains:

- 96 scenario records within each retained block (M1, M2, and M3);
- 288 scenario records across the three retained blocks;
- seven evaluated model labels per scenario;
- 2,016 model-by-scenario rows in the long-form Stage D file;
- one M1 top-three placement among 96 M1 scenarios, giving a top-three frequency of 0.0104.

No model rerun was performed to create this archive.

## File inventory

| File | Rows | Role |
|---|---:|---|
| `data/stage_d_model_group_summary.csv` | 21 | Final model-by-block summary used to verify the reported Stage D means and standard deviations for IBS, IBS_STD95, concordance, and NLS/NLL. |
| `data/stage_d_scenario_level_metrics.csv` | 2,016 | Long-form model-by-scenario Stage D archive. The first column has been given the explicit header `scenario_id`; metric values are unchanged. |
| `data/stage_b_candidate_metrics_sanitized.csv.gz` | 174,960 | Compressed development-level candidate/run archive retained for provenance. It is not the direct source for the final Chapter IV tables. The absolute HPC account prefix in `metrics_path` was replaced by `<HPC_ROOT>/`; numerical values are unchanged. |
| `checksums.sha256` | — | SHA-256 hashes for integrity verification. |

## Relationship to the dissertation

- **RQ1:** model-group averages for standardized IBS and pair-sampled concordance, plus scenario-relative rank evidence.
- **RQ2:** time-grid and Brier-curve fields in the scenario-level archive.
- **RQ3:** common-grid weighted negative log score fields.
- **RQ4:** scenario-level dispersion, mean-rank, top-three-frequency, and operating-condition summaries.

Appendix A contains the consolidated implementation and artifact crosswalk. Appendix B documents the machine-readable benchmark evidence.

## Recommended citation

Aghamie, S. O. (2026). *Supplemental synthetic benchmark data for a DeepSurv-inspired conditional discrete-time mixture-of-experts survival framework* (Version 1.0) [Data set]. GitHub. https://github.com/Sunnyblue71/dissertation-appendix-b/releases/tag/v1.0.0

## Versioning

Create a GitHub release tagged `dissertation-appendix-b-v1.0` after uploading these files. Cite that fixed release rather than the moving `main` branch.

## Data stewardship

This repository should contain only synthetic benchmark metrics and nonrestricted provenance records. Do not upload patient-level clinical data, credentials, access tokens, or restricted source data.
