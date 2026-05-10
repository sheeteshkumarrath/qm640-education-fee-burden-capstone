# Raw Data Folder

This folder is intended for storing the original raw microdata files used in the QM640 Education Fee Burden Capstone project.

## Important Note
The raw NSS and CMS microdata files are **not included** in the public GitHub repository. They must be obtained separately from the official source and stored locally in this folder before running the notebook.

This is done for the following reasons:
- the files are large
- they are official microdata files
- redistribution may be restricted by source-specific access or usage conditions

## Expected Files

Place the following files in this folder:

### NSS 75th Round
- `R75252L02-Block-3-household-characteristics.csv`
- `R75252L05-Block-5-Dducation-particulars-on-basic-course-of-the-persons-of-age-3-to-35-years-who-are-currently-attending-education.csv`
- `R75252L06-Block-6-Particulars-of-expenditure-Rs.-for-persons-of-age-3-to-35-years-who-are-currently-attending-at-pre-primary-and-above-level.csv`

### CMS-E 2025
- `CMSE80HH25.csv`
- `CMSE80PER25.csv`
- `CMSE80PERST25.csv`

## How These Files Are Used
These raw files are used in the notebook to:
- extract household-level variables
- aggregate person-level education expenditure
- merge household and expenditure records
- construct annual household consumption and education fee burden indicators
- build model-ready cleaned datasets saved in `data_processed/`

## Notebook Dependency
The main notebook:
- `notebooks/Term3_Capstone.ipynb`

expects these files to be available locally before execution.

## Recommendation
Do not rename the raw files unless you also update the file paths inside the notebook.
