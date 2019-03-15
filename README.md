# Review-copy

# Chopped - LD (Bombus and Polistes each)
Genome divided into 100k base windows, LD, mutation types/counts, and GC% calculated individually.
GC% per segment was calculated by referring back to the fasta file.
For each analysis, has adjusted and raw graphs.
Raw data are simple tally of each mutations. Adjusted are those raw numbers divided by the % fraction of the target nucleotide. (ex. S -> W mutation, number of occurances divided by GC% of the 100kbase section of genome. For W -> S, it is divided by AT%)
Looks at Odds ratios and Lambda.
** No Output files provided for less cluttered viewing of the codes.


# Ancestral Allele (one file contains both Bombus and Polistes)
Very first work. Looks at the entire vcf and determines ancestral allele and derived allele based on Alternative Allele Frequency (AF). Defines which mutations are SW and which are WS. Makes a overall tally based on mutation type and frequency, generated a stacked bar graph. Also have raw and adjusted figures. Adjustment made with genome wide GC% based off NCBI's genome database.

# GC Content
Calculation of proportion of GC per 100k segments and compared it to mean R^2 of the corresponding segments.

# Polistes - Intergenic
Example file for annotated segment Odds ratio. Both Bombus and Polistes had their SNPs containing vcfs divdied into Synonymous, Non-Synonymous, Intergeic, and Intronic categories. The procedure done in 'Ancestral Allele Call' was repeated and OR was calculated per segment.
  ** No intragenic file.
