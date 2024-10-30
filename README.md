# dsp_nfcore_rnaseq

## RNA sequencing analysis pipeline

nf-core/rnaseq is a bioinformatics pipeline that can be used to analyse RNA sequencing data obtained from organisms with a reference genome and annotation. It takes a samplesheet and FASTQ files as input, performs quality control (QC), trimming and (pseudo-)alignment, and produces a gene expression matrix and extensive QC report.

You can find a more exhaustive description and running instructions in here: https://nf-co.re/taxprofiler/1.1.7

Here we provide with a small manual to how to prepare, for running the pipeline and running it in the Microsoft Azure environment.

## Create samplesheet.csv as:
```
sample,run_accession,instrument_platform,fastq_1,fastq_2,fasta
2612,run1,ILLUMINA,2612_run1_R1.fq.gz,,
2612,run2,ILLUMINA,2612_run2_R1.fq.gz,,
2612,run3,ILLUMINA,2612_run3_R1.fq.gz,2612_run3_R2.fq.gz,
...
```