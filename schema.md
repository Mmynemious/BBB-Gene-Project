# BBB Gene Dataset Schema

This repository standardizes blood–brain barrier (BBB) gene expression datasets into a common format for reproducible analysis.

## Core Columns

- **GeneSymbol**  
  Official HGNC gene symbol.

- **ExpressionValue**  
  Normalized expression level (units vary by source dataset; see Notes).

- **Condition**  
  Experimental condition (e.g., control, inflammation, knockout).

- **Source**  
  Publication or dataset reference (e.g., Daneman2010, Munji2019).

- **Notes**  
  Dataset-specific annotations, caveats, or preprocessing details.

## Directory Structure

- `raw_data/` → Original datasets as published.  
- `processed/` → Cleaned and standardized tables following this schema.  
- `scripts/` → R/Python scripts used for cleaning and formatting.  
- `docs/` → Documentation files (including this schema).

## Usage Notes

- All datasets are harmonized to the above schema for cross-study comparison.  
- Raw values are preserved for transparency.  
- Cleaning scripts document every transformation step.  
