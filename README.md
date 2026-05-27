# Reference genomes and structural variants comparison in populations of *Caretta caretta*

This repository contains the pipelines and workflows developed for my Master’s Thesis on comparative genomics in the loggerhead sea turtle (*Caretta caretta*). The project includes whole-genome alignments, dotplot visualization, genetic distance analyses, synteny analyses, and structural variant detection across different Regional Management Units (RMUs).

## Repository structure

The `TFM/` folder contains six pipeline files describing the analyses performed throughout the project. These files are not directly executable scripts, but detailed step-by-step workflows including terminal commands and embedded R/Python scripts.

Embedded scripts are delimited by:

```text
---
script
---
```

Some commands are also intended to be executed directly in the Linux terminal without standalone scripts.

## Pipelines

`how_to_mapping`

Mapping of the 14 trimmed *Caretta caretta* samples against the Atlantic (RMU: NEA) and Pacific (RMU: NP) reference genomes, generating sorted BAM files.

`how_to_genotyping`

Variant calling and genotyping workflow using the three reference genomes: Mediterranean (MED), Atlantic (NEA), and Pacific (NP). Includes VCF generation, filtering, and preparation for profile visualization to explore potential inversion regions.

`how_to_Manta`

Structural variant detection using Manta and SURVIVOR across the 14 samples mapped against the three assemblies.

`how_to_COMPARISON_THREE_GENOMES_DOTPLOTS`

Pairwise comparison of the three reference genomes through whole-genome alignments and dotplot generation to assess synteny.

`how_to_COMPARISON_THREE_GENOMES_SYRI_PLOTSR`

Pairwise synteny and structural rearrangement analyses using Syri and plotsr to support dotplot-based observations.

`how_to_COMPARISON_THREE_GENOMES_GENETIC_DISTANCE`

Pairwise comparison of the three reference genomes to obtain a general overview of genetic distance patterns.

## Softwares used
- minimap2
- samtools
- bcftools
- Manta
- SURVIVOR
- Syri
- plotsr
- R
- Python
