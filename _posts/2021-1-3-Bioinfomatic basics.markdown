---
layout: post
title: "Introduction to Bioinformatics"
date:  2021-1-4
category: data basics

---


# Introduction into Bioinfomatics

**Bioinformatics** is a type of biology that studies the patterns of genomic sequences of DNA, RNA, and proteins in animal, bacterial or viral organisms. 
Bioinfomatics discoveres how genomic codes produce functional output in cells. How different layers of genetic codes relate to each other. How are these codes responsible for development, age and disease? If these are new concepts to you, I suggest reading the [NIH Human Genome Introduction](https://www.genome.gov/About-Genomics/Introduction-to-Genomics) to learn how these molecules are composed of repeating strucutures producing a genetic codes

Genomic infomation is handy for understanding the inner working of cells, but also to intentify organisms in a mixed population. This is especially relevant to describing microbiomes which are composed of hundreds of different species of [microbes](https://en.wikipedia.org/wiki/Microorganism). 

# Where does the data come from? 
Simply, genomics data comes from labs. Genomic data is derived either from experimental trials, like measuring the mRNA after a chemical treatment, or directly from patients samples, which can be used to understand the genetic contribution to pathology. 

What's so exciting about bioinformatics is **you don't need a lab to access genomic data**. Many datasets are publically available online repositories, such as 

-[NCBI Genomic Expression Omnibus](https://www.ncbi.nlm.nih.gov/geo/)

-[The Cancer Genome Atlas](https://www.cancer.gov/about-nci/organization/ccg/research/structural-genomics/tcga)

-[NCBI GenBank](https://www.ncbi.nlm.nih.gov/genbank/)

-[International Cancer Genome Consortium](https://daco.icgc.org/)

-[cBioPortal](http://cbioportal.org)

-[Cancer Cell Line Encyclopedia](https://portals.broadinstitute.org/ccle/)

-[ENCODE, Encyclopedia of DNA Elements](https://www.encodeproject.org/)

The repositories are either government funded or privately funded, but they all are free to download data. Where data is stored largely depends on the size of the data. It can be stored either locally, cloud computing or deposited into large data storing initatives, like in the list above. Where data is stored depends on whether data is published and/or contains sensitive patient information. 

# How to store and open genomic data

Data is stored either in file, database or an online application (API). A few typical file formats are plain text, tab-delimited format (.txt), binary files (.BAM), web-based markup language (.xml), and many more. 

Sequence files are imported into a platform for visualization and analysis. 

If you want to **visualize** sequences, you can use a genome browser like [ENSEMBL](https://useast.ensembl.org/index.html), [UCSC Genome Browser](https://genome.ucsc.edu/), [NCBI Genome Data Viewer](https://www.ncbi.nlm.nih.gov/genome/gdv/), and [3D Genome Browser for exploring chromatin interactions](http://3dgenome.fsm.northwestern.edu/). Genome browsers are very useful, but limited in analytical power. For deeper bioinfomatic **analysis**, one must make use of programming languages like R, Python, and Unix. In this blog, I'll be describing operations in R. 

# The future of genomic data storage
[The average human genome is about 100GB of storage space](https://www.technologyrecord.com/Article/microsoft-genomics-service-launched-to-accelerate-healthcare-innovation-63673)

 
