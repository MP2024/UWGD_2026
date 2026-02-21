# Task 8. Read depth (DP) by Transitions and Transversions 

This pipeline allows assessing difference in the read depth (DP) between transitions and transversions. The pipeline comprises of two parts—data extraction (produces a tsv file with two columns – DP and info about mutation type: transition/transversion) and data analysis (creates a plot showing how is the DP distributed within the mutation types.

## 1. Data Extraction (Bash)

The data extraction part is represented by a script workflow.sh. To execute the script use: \
`./workflow.sh`

### Workflow.sh
This script takes a vcf file as an input and produces a tsv file with two columns&mdash;DP and mutation type&mdash;as its output. During this process, several thing are done with the original vcf folder:

#### 1. Variables Definition
The filename and point mutation types (transition, transversion) are defined within this section.

> [!NOTE]
> luscinia_vars.vcf.gz file in the folder data is set as the default input. 

#### 2. DP Extraction


#### 3. Mutation type extraction


#### 4. Final Check


#### 5. Merging the DP and mutation type data


#### 6. Removing the DP and mutation type tsv files





## 2. Data Analysis (R)
