# Reproducibility Guide

1. Keep the original CSV files in `data/raw/` and cleaned files in `data/cleaned/`.
2. Install dependencies listed in `requirements.txt`.
3. Run inspection, quality checks, cleaning and validation scripts in order.
4. Run EDA, business analysis and RFM scripts.
5. Rebuild charts and reports if source data changes.
6. Record any changed assumptions in this folder.

The scripts should be run from the project's `python/` directory, with `config.py` resolving paths relative to the project root.
