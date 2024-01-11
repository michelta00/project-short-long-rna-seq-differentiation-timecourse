# Comparison of Time-Course Short and Long Read RNA-seq Data
This is a repository for STA426 AS24 project.
# Table of contents
1. [Abstract](#abstract)
2. [Code availability](#code)
    * [Structure](#structure)
6. [Usage](#usage)
    * [Software requirements](#Software)
    * [Installation](#installation)
7. [References](#references)


## Abstract <a name="abstract"></a>
The long-read RNA-sequencing methods enable sequencing with long read lengths for RNA isoform identification and quantification as they can cover the splice junctions. However, these platforms cannot attain the necessary read depths since they suffer from low read depths/throughputs. The short-read sequencing technologies are high-throughput, but due to short read lengths they cannot cover splice sites. In this project,  a newly introduced method for long-read sequencing of transcript isoforms based on ISO-seq, multiplexed arrays isoform sequencing (MAS-ISO-seq)  introduced by Al’Khafaji et al (2023), was tested and compared to the common Illumina (short-read sequencing) RNA-seq protocol. A  MAS-ISO-seq relies on the concatenation of cDNA fragments into longer sequence libraries with a narrow length distribution which then can be sequenced by PacBio. The data sets contain samples from WTC-11 cells (induced pluripotent stem cells) that underwent a directed differentiation from pluripotent stem cells to hemogenic endothelial cells for 6 days with 1-3 replicates each day. These samples were then sequenced using both the PacBio and Illumina platforms and were subsequently quantified with Bambu in the case of the PacBio sequence data and with Salmon in the case of Illumina sequence data. The quantification was performed using 4 different novel discovery rate (NDR) thresholds, which approximate the proportion of novel transcripts to control the balance between the sensitivity and the precision of the transcript discovery. The obtained data sets were finally compared in an exploratory data analysis (EDA), a differential gene expression (DGE) analysis and a differential transcript usage (DTU) analysis to explore the performance of the MAS-ISO-seq protocol compared to Illumina sequencing, which has been used and thus underwent optimization for much longer.
## Code availability <a name="code"></a>
The detailed analysis can be found in the `code` folder. 
## Structure <a name="structure"></a>
The project has the following structure:

```
project-short-long-rna-seq-differentiation-timecourse
│   README.md
│   report.qmd
|   report.html  
│
└───code
│   │
│   └───
│   │
│   └───

└───plots
│   │
│   └───
└───data
│   │
│   └───


```

 # Usage <a name="usage"></a>

All code was run on **R 4.3.1** on **Ubuntu 23.04** and **macOS Sonoma 14.2.1**. 

## Software Requirements <a name="Software"></a>

* <img src=https://github.com/simple-icons/simple-icons/blob/develop/icons/python.svg height=20> R 4.3.1
* <img src=https://github.com/simple-icons/simple-icons/blob/develop/icons/ubuntu.svg height = 20> Ubuntu 23.04
* <img src=https://github.com/simple-icons/simple-icons/blob/develop/icons/macos.svg height=20> macOS Sonoma 14.2.1

# References <a name="references"></a>

1. Al’Khafaji AM, Smith JT, Garimella KV, Babadi M, Popic V, Sade-Feldman M, Gatzen M, Sarkizova S, Schwartz MA, Blaum EM et al (2023) High-throughput RNA isoform sequencing using programmed cDNA concatenation. Nat Biotechnol
