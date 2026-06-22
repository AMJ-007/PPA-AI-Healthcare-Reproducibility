# Privacy-Preserving Agentic AI for Healthcare: Reproducibility Package

This repository provides the reproducibility materials for the study:

**Privacy-Preserving Agentic AI for Healthcare: A Homomorphic Encryption-Based Framework for Secure and Policy-Governed Decision Intelligence**

The package contains the implementation, experimental outputs, figures, environment specifications, and execution notes used to evaluate a CKKS-based privacy-preserving agentic AI framework for secure healthcare decision intelligence.

## Study Summary

The framework combines:

- CKKS homomorphic encryption using TenSEAL;
- encrypted inference over protected patient feature vectors;
- a policy-aware agentic controller for governed workflow execution;
- evaluation using the UCI Heart Disease dataset.

The experimental evaluation used a full held-out test set of 60 samples.

## Reported Results

| Metric | Value |
|---|---:|
| Encrypted Accuracy | 83.33% |
| Precision | 84.62% |
| Recall | 78.57% |
| F1-score | 81.48% |
| Specificity | 87.50% |
| Balanced Accuracy | 83.04% |
| Plaintext ROC-AUC | 0.9498 |
| Encrypted ROC-AUC | 0.9495 |
| Average Encryption Time | 0.01095 s |
| Average Encrypted Inference Time | 0.03382 s |
| Total Secure Processing Time | 0.04477 s |

## Repository Structure

data/           Public UCI Heart Disease data and processed dataset
figures/        Final full-test evaluation figures
notebooks/      Google Colab notebook for encrypted agentic inference
requirements/   Python environment and package requirements
results/        Full-test predictions and final metrics summary
runtime_logs/   Execution environment and reported runtime information


### Reproduction:
Create a Python environment using the files in requirements/.
Open notebooks/01_colab_agentic_ckks_uci_heart_experiment.ipynb in Google Colab.
Install the listed dependencies.
Run the notebook sequentially from top to bottom.
Compare generated outputs with the files in results/ and figures/.

**Notes
The dataset is derived from the publicly available UCI Heart Disease dataset.
Runtime measurements can vary across Google Colab sessions and allocated CPU resources.
The repository contains no patient-identifiable data, private manuscript files, editorial correspondence, or credentials.
Citation


If you use this package, please cite the associated manuscript:

M. J. Abdullahi, I. S. Emmanuel, G. Tripathi, and A. K. Ball, “Privacy-Preserving Agentic AI for Healthcare: A Homomorphic Encryption-Based Framework for Secure and Policy-Governed Decision Intelligence,” submitted for publication.

#License
This repository is provided for academic research and reproducibility purposes.

