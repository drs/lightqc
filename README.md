# LightQC

LightQC is a lightweight Nanopore/PacBio reads quality control tool that relies on FASTQ files to evaluate the quality for one dataset or compare multiple datasets. 

LightQC computes some metrics from the reads file such as PHRED score and reads length as well as from the alignment of the reads against a reference genome.

## Installation 

This software only depends on Python 3 with some additionnal packages. 

1. Install the dependancies with pip. 

```
pip install pandas, numpy, scipy, plotly
```

2. Install Minimap2 as described in [Minimap2 Installation](https://github.com/lh3/minimap2#install). Minimap2 must be avaiable on the PATH for LightQC. 

3. Download this script and add the script location to the path or move the script to a localisation in your path (such as $HOME/bin). 

```
git clone https://github.com/drs/LightQC
```

## Usage 

Typical usage : 

```
LightQC -g genome.fasta -r reads.fastq -x nanopore -o LightQC.html 
```

## Feature Request 

LightQC is still under active development. Feel free to submit any feature request through GitHub Issues tracker or by email. 

## Alternative Tools 

While this tools aims at providing a fast and lightweight all-in-one solution for Nanopore/PacBio reads quality control, alternatives tools offer different interesting features :  

- [AlignQC](https://github.com/jason-weirather/AlignQC)  
- [LongQC](https://github.com/yfukasawa/LongQC)  
- [NanoOK](https://nanook.readthedocs.io/en/latest/)  
- [NanoPlot](https://github.com/wdecoster/NanoPlot)  
- [pycoQC](https://github.com/tleonardi/pycoQC)  

Some parts of this tools are heavily inspired from these software, mostly from pycoQC. 
