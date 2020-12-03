# INTRODUCTION
In this folder the code accompanying the manuscript:

### Genetic heterogeneity and subtypes of major depression

Thuy-Dung Nguyen, M.Sc.(1,2); Arvid Harder, B.Sc.(1); Ying Xiong, M.Sc.(1); Kaarina Kowalec, Ph.D.(1,3); Sara Hägg, Ph.D.(1); Na Cai, Ph.D.(4), Ralf Kuja-Halkola, Ph.D.(1); Christina Dalman, M.D.(2); Patrick F Sullivan, M.D. FRANZCP(1,5); Yi Lu, Ph.D.(1,2)
1.	Department of Medical Epidemiology and Biostatistics, Karolinska Institutet, Stockholm, Sweden
2.	Department of Global Public Health, Karolinska Institute, Stockholm, Sweden
3.	College of Pharmacy, University of Manitoba, Winnipeg, Canada
4.	Helmholtz Pioneer Campus, Helmholtz Zentrum München, Neuherberg, Germany
5.	Department of Genetics and Psychiatry, University of North Carolina, Chapel Hill, NC, USA

# DERIVE PHENOTYPE IN UKB
## EXTRACT DATA UKB
The code in the UKB_variable_extraction.Rmd was used to extract data from UKB original datasets.
In this file, you can find the list of variable which were stored in each dataset mentioned in the section DERIVE MD CASES, CONTROLS, EXCLUSION CRITERIA and DERIVE MD SUBTYPES.
If having access the UKB datasets, you can use these code to extract variable out into small raw datasets. Then, use those raw datasets as input dataset to derive variables.

## DERIVE MD CASES, CONTROLS, EXCLUSION CRITERIA
The code in Derive_MD_case_control.Rmd was used to derive MD cases, control and exclusion criteria. 
Input data are mentioned in the EXTRACT DATA UKB.

## DERIVE MD SUBTYPES
The code in Derive_subtype.Rmd was used to derive MD subtypes for the study.
Input data are mentioned in the EXTRACT DATA UKB.

## PIPILINE FOR GWAS, ESTIMATING SNP-HERITABILITY AND GENETIC CORRELATION
After derivinng phenotypes, we constructed phenotype dataset for each subtype, and use this pipeline to conduct GWAS and estimating SNP-heritability, genetic correlations.
Instruction on:
- How to conduct GWAS using fastGWA including how to prepare phenotype data could be found here: https://cnsgenomics.com/software/gcta/#fastGWA
- How to install LDSC and estimate SNP-heritability could be found here: https://github.com/bulik/ldsc
- How to install HDL and estimate genetic correlation could be found here: https://github.com/zhenin/HDL
