# RNA-seq-Analysis-with-R

In general, the analysis of differential expression for RNA-seq is divided into two steps (each one that in turn includes other steps):

QA:
- Count of gene-associated reads
- Normalization
- Unsupervised cluster analysis

Differential Expression Analysis
- Modeling of raw counts for each gene
- Reduced log2 fold changes
- Test the differential expression

## Case study

In this case we are going to work with a dataset used by the article by Gerarduzzi et al., 2017 (DOI: 10.1172/jci.insight.90299). Basically, they want to know why mice overexpressing the Smoc2 gene are more likely to develop renal fibrosis. In this case, two sample groups are being tested:
- 3 Mice without fibrosis and with overexpression of Smoc2
- 4 mice with fibrosis and with overexpression of Smoc2
Essentially, one wants to know if gene expression is differential between groups.

First we need the gene-associated read counts and the associated sample metadata
