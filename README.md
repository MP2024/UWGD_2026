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
> The _luscinia_vars.vcf.gz_ file in the folder _data_ is set as the default input.

#### 2. DP Extraction
Using functions grep and awk, the DP data from individual entries (lines) are extracted into the dp.tsv file. The awk code (using functions match and substr) was based on [Mark Needham's blog post](https://www.markhneedham.com/blog/2013/06/26/unixawk-extracting-substring-using-a-regular-expression-with-capture-groups/). 

#### 3. Mutation type extraction
Using functions grep and awk, the mutation type data were extracted into the mutation_type.tsv file. There are four possible outputs for each entry – transition, transversion, NA1 (indels or locī) or NA2 (undefined single-nucleotide exchange, should not exist in our data)

#### 4. Final Check


#### 5. Merging the DP and mutation type data


#### 6. Removing the DP and mutation type tsv files





## 2. Data Analysis (R)
