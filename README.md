# Task 8. Read depth (DP) by Transitions and Transversions 

This pipeline allows assessing difference in the read depth (DP) between transitions and transversions. The pipeline comprises of two parts—data extraction (produces a tsv file with two columns – DP and info about mutation type: transition/transversion) and data analysis (creates a plot showing how is the DP distributed within the mutation types.

## 1. Data Extraction (Bash)

The data extraction part is represented by a script workflow.sh. To execute the script use: \
`./workflow.sh`

### Workflow.sh
This script takes a vcf file as an input and produces a tsv file with two columns&mdash;DP and mutation type&mdash;as its output.

## 2. Data Analysis (R)
