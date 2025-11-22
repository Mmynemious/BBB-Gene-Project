# BBB-Gene-Project

This repository contains curated endothelial gene expression datasets from key publications.
Each dataset is processed individually into a standardized schema before being merged into a master file.

## Structure
- raw_data/: Original datasets
- processed/: Cleaned datasets
- scripts/: R scripts for processing
- docs/: Schema documentation


### Munji2019 dataset handling

The original `Munji2019_cleaned.csv` exceeded GitHub’s 2 GB per-file limit for Git LFS.  
It has been split into ~500 MB chunks:

- `processed/Munji2019_part_aa`
- `processed/Munji2019_part_ab`
- `processed/Munji2019_part_ac`
- `processed/Munji2019_part_ad`
- `processed/Munji2019_part_ae`

To reconstruct the full dataset locally, run:

```bash
cat processed/Munji2019_part_* > processed/Munji2019_cleaned.csv
