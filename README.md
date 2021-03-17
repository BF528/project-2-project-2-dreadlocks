# Project Description
The goal of this project was to reproduce part of the results of the study Transcriptional Reversion of Cardiac Myocyte Fate During Mammalian Cardiac Regenerationdone by O’Meara et al, and to learn and practice using the bioinforamtics tools implemented in this study. <br/>
<br/>
The objectives of the original study was to determine if myocytes revert the transcriptional phenotype to a less differentiated state during regeneration and to systematically interrogate the transcriptional data to identify and validate potential regulators of this process.<br/>
<br/>
In this project we downloaded RNA-Seq sequencing data from GEO, performed quality control, aligned the reads to mouse genome mm9, quantified gene expression, and identified differentially expressed genes associated with myocyte differentiation.<br/>
<br/>
O’Meara et al. Transcriptional Reversion of Cardiac Myocyte Fate During Mammalian Cardiac Regeneration. Circ Res. Feb 2015. PMID: 25477501<br/>


# Contributors
- Data Curator: Sarah Zhang (@zhiyu-zz) zzyu@bu.edu<br/>
- Programmer: Jianfeng Ke (@jke20) jke@bu.edu<br/>
- Analyst: Huisiyu Yu (@yuhuisiyu) yhsy@bu.edu<br/>
- Biologist: Yu Zhong (@yuzhong1997) yuzhong@bu.edu<br/>

# Repository Contents
## Data Curator
### run_extract.qsub
- Dependencies: SRA toolkit<br/>
- Execution: `qsub run_extract.qsub`<br/>
- Outputs: P0_1_1.fastq, P0_1_2.fastq<br/>
- Convert sample from sra to fastq format.<br/>

### run_qc.qsub
- Dependencies: FastQC<br/>
- Execution: `qsub run_qc.qsub`<br/>
- Outputs: P0_1_1_fastqc.html, P0_1_2_fastqc.html<br/>
- Generate quality control reports<br/>

## Programmer
### run_tophat.qsub
- Dependencies: TOPHAT<br/>
- 
## Analyst
## Biologist
- Script: `biologist.R`<br/>
- Output: see project report Figure 7 and 8<br/>
- 
