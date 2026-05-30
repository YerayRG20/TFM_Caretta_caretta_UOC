# Reference genomes and structural variants comparison in populations of *Caretta caretta*

This repository contains the pipelines and workflows developed for my Master’s Thesis on comparative genomics in the loggerhead sea turtle (*Caretta caretta*). The project includes whole-genome alignments, dotplot visualization, genetic distance analyses, synteny analyses, and structural variant detection across different Regional Management Units (RMUs).

## Repository structure

The repository is organized into different folders according to the type of material included.

The `pipelines/` folder contains six pipeline files describing the analyses performed throughout this project. These files are not directly executable scripts, but detailed step-by-step workflows including terminal commands and embedded R/Python scripts.

Embedded scripts are delimited by:

```text
---
script
---
```

Some commands are also intended to be executed directly in the Linux terminal without standalone scripts.

The `figures/` folder contains high-resolution versions of the figures included in the thesis. These files are provided to facilitate detailed visualization of genomic comparisons, structural rearrangement analyses, and other graphical outputs that may appear reduced in size within the report.

The `supplementary_figures/` folder contains additional supplementary visualizations that were not included directly in the thesis due to their large size.

## Pipelines

The following pipeline documents are located in the `pipelines/` folder:

`how_to_mapping`

Mapping of the 14 trimmed *Caretta caretta* samples against the Atlantic (RMU: NEA) and Pacific (RMU: NP) reference genomes, generating sorted BAM files.

`how_to_genotyping`

Variant calling and genotyping workflow using the three reference genomes: Mediterranean (MED), Atlantic (NEA), and Pacific (NP). Includes VCF generation, filtering, and preparation for profile visualization to explore potential inversion regions.

`how_to_Manta`

Structural variant detection using Manta and SURVIVOR across the 14 samples mapped against the three assemblies.

`how_to_three_genome_dotplots`

Pairwise comparison of the three reference genomes through whole-genome alignments and dotplot generation to assess synteny.

`how_to_three_genome_syri`

Pairwise synteny and structural rearrangement analyses using SyRI and plotsr to support dotplot-based observations.

`how_to_three_genome_genetic_distance`

Pairwise comparison of the three reference genomes to obtain a general overview of genetic distance patterns.

## Figures

High-resolution versions of all figures included in the thesis can be found in the `figures/` folder. These files correspond to the figures presented throughout the report and are provided to allow detailed inspection of genomic patterns, dotplots, synteny visualizations, genetic distance analyses, and structural variant results.

## Supplementary figures

The repository also includes a `supplementary_figures/` folder containing complete chromosome-by-chromosome homozygosity profile visualizations generated for the three reference assemblies:

- Mediterranean (MED)
- Atlantic (NEA)
- Pacific (NP)

These PDF files were used for exploratory visualization of potential inversion-related patterns across the different assemblies and are provided as supplementary material due to their large size.

## Software used
- Minimap2
- SAMtools
- BCFtools
- VCFtools
- HISAT2
- FastQC
- Trimmomatic
- iDIG
- Picard
- Manta
- SURVIVOR
- SyRI
- plotsr
- R
- Python
