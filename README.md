# Large-scale Genetic Characterization of Parkinson’s disease in the African and African admixed Populations

`GP2 ❤️ Open Science 😍`

Pending DOI

**Last Updated:** December 2024

## Summary
This repository contains all analyses for the manuscript titled ***"Large-scale genetic characterization of Parkinson’s disease in the African and African admixed populations"***. This study represents the largest sequencing-based characterization of potentially disease-causing protein-altering and splicing mutations in 710 cases and 11,827 controls from genetically predicted African or African admixed populations.

---

### Data Statement 
* Results were generated using
  - GP2 data release 8 (controlled-tier access; DOI 10.5281/zenodo.13755496)  
  - All of Us (AoU) genomic data release 7 (controlled-tier access)

### Datasets

| Dataset   | Release / Version | Resource URL                                                                                                                | Notes                                                                             |
|-----------|-------------------|-----------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------|
| All of Us | Release 7         | [https://allofus.nih.gov/](https://allofus.nih.gov/) <br/> [https://workbench.researchallofus.org/](https://workbench.researchallofus.org/)   | Controlled-tier data used in this study                                           |
| GP2       | Release 8         | [https://gp2.org/the-components-of-gp2s-8th-data-release/](https://gp2.org/the-components-of-gp2s-8th-data-release/)                          | Access-controlled data used in this study                                         |
| BLAACPD   | .        | [https://www.blaacpd.org/DJYD/](https://www.blaacpd.org/DJYD/)                                                                                 | Cohort focusing on African / African admixed populations with PD                  |

---

### Repository Orientation


```
analyses/ 
├── 00_Annotation_AFR_PDexome.ipynb
├── 01_GP2_AfricanPD.ipynb
└── 02_Annotation_AFR_PDexome.ipynb
```

---

### Analysis Notebooks

**Languages**: Python and bash

| **Notebook(s)**                   | **Description**                                                                                                                                                                                              |
|:---------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| `00_Annotation_AFR_PDexome.ipynb` | Annotation of variants identified in GP2 WGS African ancestry cohort and in PD GENEration clinical exomes.                                                                                                   |
| `01_GP2_AfricanPD.ipynb`          | Analysis of PD genes in GP2 cases and controls of African and African admixed ancestries (release 8). <br/> Includes extracting individuals, recoding VCFs, and evaluating the intronic rs3115534-G variant. |
| `02_Annotation_AFR_PDexome.ipynb` | Extraction of African/admixed PD cases and controls from All of Us WGS data (release 7), recoding VCFs, and analysis of the intronic *GBA* rs3115534-G variant.                                              |


> **Note**: For more details on each notebook’s usage, refer to the introduction and documented code sections contained within each respective `.ipynb`.

---

### Software

| Software            | Version(s)     | Resource URL                                                                                                                                                                 | RRID              | Notes                                                         |
|---------------------|----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|---------------------------------------------------------------|
| ANNOVAR             | 2020-06-08     | [http://www.openbioinformatics.org/annovar/](http://www.openbioinformatics.org/annovar/)                                                                                      | RRID:SCR_012821   | Genetic annotation software                                   |
| BCFtools            | 1.17 | [https://samtools.github.io/bcftools/bcftools.html](https://samtools.github.io/bcftools/bcftools.html)                                                                       | RRID:SCR_002105   | Used for variant calling file (VCF) manipulation              |
| GBA Gauchian Caller | 1.0  | [https://github.com/Illumina/Gauchian](https://github.com/Illumina/Gauchian)                                                                                                  | . | Used for specialized *GBA* analyses                           |
| PLINK / PLINK2      | 1.9 & 2.0      | [https://zzz.bwh.harvard.edu/plink/plink2.shtml](https://zzz.bwh.harvard.edu/plink/plink2.shtml) <br/> [https://www.cog-genomics.org/plink2](https://www.cog-genomics.org/plink2) | RRID:SCR_001757   | Used for genetic analyses                                     |                           |
