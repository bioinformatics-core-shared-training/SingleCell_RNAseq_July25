# Introduction to single-cell RNA-seq data analysis

### 10th, 11th, 14th July 2025 || 09:30 - 17:00
#### In-person, Craik-Marshall training room ([map](https://www.google.co.uk/maps?hl=en-GB&q=Craik-Marshall+Building,+Downing+Site,+Cambridge&source=calendar))

![](UnivCambridge_ScRnaSeqIntro_Base/Images/uniOfCamCrukLogos.png)

## Instructors

- Abbi Edwards (CRUK)
- Chandra Chilamakuri (CRUK)
- Ramy Ragheb (Stem Cell Institute)
- Daianna Gonzales Padilla (Sanger)
- Guest Speaker: Kasia Kania (Cosyne Therapeutics)

## Outline

This workshop is aimed at biologists interested in learning how to perform
standard single-cell RNA-seq analyses.

This will focus on the droplet-based assay by 10X genomics and include running
the accompanying `cellranger` pipeline to align reads to a genome reference and
count the number of read per gene, reading the count data into R, quality control,
normalisation, data set integration, clustering and identification of cluster
marker genes, as well as differential expression and abundance analyses.
You will also learn how to generate common plots for analysis and visualisation
of gene expression data, such as TSNE, UMAP and violin plots.

> ## Prerequisites
>
> __**Some basic experience of using a UNIX/LINUX command line is assumed**__
>
> __**Some R knowledge is assumed and essential. Without it, you
> will struggle on this course.**__
> If you are not familiar with the R statistical programming language we
> strongly encourage you to work through an introductory R course before
> attempting these materials.
> We recommend our [Introduction to R course](https://bioinformatics-core-shared-training.github.io/r-intro/).

## Data

* The course data is based on '[CaronBourque2020](https://www.nature.com/articles/s41598-020-64929-x)'
  relating to pediatric leukemia, with four sample types, including:
  * pediatric Bone Marrow Mononuclear Cells (PBMMCs)
  * three tumour types: ETV6-RUNX1, HHD, PRE-T  
* The data used in the course can be [downloaded from Dropbox](https://www.dropbox.com/scl/fo/9uu4iuapr60jfu2bvggdz/AFaCOxLcO5aKrqzHiEUD1ao?rlkey=zqkpbux9q0yak8e0ok59djfr0&st=inmhk174&dl=0). Please note that:
  * these data have been processed for teaching purposes and are therefore not suitable for research use;
  * all the data is provided on our training machines, you don't need to download it to attend the course.

## Schedule

**PDF of materials:** if you want a PDF version of the materials go to the "Print" option on your browser and select "Print to PDF" (all major browsers have this functionality).

### Day 1


* 09:30 - 09:45 **Welcome** - Hugo
* 09:45 - 10:30 **Introduction to Single Cell Technologies** - Katarzyna Kania
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/01_Introduction.pdf)
* 10:30 - 10:44 **Preamble**: data set and workflow - Abbi
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/02_PreambleSlides.html)
* 10:45 - 11:00 - **Break**
* 11:00 - 12:30 Library structure, **cellranger** for alignment and cell calling - Abbi
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/03_CellRangerSlides.html) \([pdf](UnivCambridge_ScRnaSeqIntro_Base/Slides/03_CellRangerSlides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/03_CellRanger.html)
* 12:30 - 13:30 **Lunch break**
* 13:30 - 17:00 **QC and exploratory analysis** - Chandra
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/04_QualityControlSlides.html) \([pdf](UnivCambridge_ScRnaSeqIntro_Base/Slides/04_QualityControlSlides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/04_Preprocessing_And_QC.html)
        <!-- + [Demo live script](live_scripts/04_demonstration_live_script.R) -->
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/04_Preprocessing_And_QC.Exercise.html)  
       <!-- + [Exercise live script](live_scripts/04_exercise_live_script.R) -->

### Day 2


* 09:30 - 09:40 **Recap** - Chandra
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/00_Day1_Recap.html)
* 09:40 - 12:30 **Normalisation** - Chandra
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/05_NormalisationSlides.html) \([pdf](UnivCambridge_ScRnaSeqIntro_Base/Slides/05_NormalisationSlides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/05_Normalisation.html)    
    + [Practical](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/05_Normalisation_exercises.html)
* 12:30 - 13:30 **lunch break**
* 13:30 - 15:25 **Feature selection and dimensionality reduction** - Ramy
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/06_FeatureSelectionAndDimensionalityReduction_slides.html) \([pdf](UnivCambridge_ScRnaSeqIntro_Base/Slides/06_FeatureSelectionAndDimensionalityReduction_slides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/06_FeatureSelectionAndDimensionalityReduction.html)
* 15:25 - 15:35 10 min **break**
* 15:35 - 17:30 **Batch correction and data set integration** - Abbi
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/07_DataIntegrationAndBatchCorrectionSlides.html) \([pdf](UnivCambridge_ScRnaSeqIntro_Base/Slides/07_DataIntegrationAndBatchCorrectionSlides.pdf)\)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/07_Dataset_Integration.html)

### Day 3

* 09:30 - 09:40 Recap - Abbi
* 09:40 - 11:05 **Cell clustering** - Abbi
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/08_ClusteringSlides.html)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/08_Clustering.html)
* 11:05 - 11:15 10 min **break**
* 11:15 - 12:30 **Identification of cluster marker genes** - Ramy
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/09_ClusterMarkerGenes.html)
    + [Demonstration](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/09_Cluster_Marker_Genes.html)
* 12:30 - 13:30 **lunch break**
* 13:30 - 17.30 **Differential Expression and Abundance Analysis** - Chandra
    + [Slides](UnivCambridge_ScRnaSeqIntro_Base/Slides/10_DifferentialExpressionAndAbundance.pdf) 
    + [Demonstration - Differential Expression](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/10_Differential_Expression.html)
    + [Demonstration - Differential Abundance](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/11_Differential_Abundance.html)


## Extended Materials

* **Seurat** walkthrough:
  * Part 1: [Data pre-processing](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/101-seurat_part1.html)
  * Part 2: [Cell clustering and annotation](UnivCambridge_ScRnaSeqIntro_Base/Markdowns/101-seurat_part2.html)


## Software Installation

You can make use of the computer environment provided for the course, which is ready for use and have the necessary data & software installed.
However, if you want to run the analysis on your own computer, you can follow these instructions.

* Download and install R: https://cloud.r-project.org/
  * (Windows users only): Download and install RTools: https://cran.r-project.org/bin/windows/Rtools/
* Download and install RStudio: https://www.rstudio.com/products/rstudio/download/#download
* Open RStudio and run the following commands from the console:
    ```r
    install.packages("BiocManager")
    BiocManager::install(c("AnnotationHub", "BiocParallel", "BiocSingular", "DropletUtils", "PCAtools", "batchelor", "bluster", "cluster", "clustree", "dynamicTreeCut", "edgeR", "ensembldb", "ggplot2", "igraph", "patchwork", "pheatmap", "scater", "scran", "tidyverse", "miloR", "robustbase", "sctransform", "Seurat"))
    ```

For Cellranger, you will need to use a Linux machine.
See the [installation instructions from 10x Genomics](https://support.10xgenomics.com/single-cell-gene-expression/software/pipelines/latest/installation).


## Acknowledgments:

Much of the material in this course has been derived from the demonstrations found in
[OSCA book](https://bioconductor.org/books/release/OSCA/)
and the [Hemberg Group course materials](https://www.singlecellcourse.org/). Additional material concerning `miloR` has been based on the [demonstration from the Marioni Lab](https://marionilab.github.io/miloR/articles/milo_demo.html).

The materials have been contributed to by many individuals over the last 2 years, including:

Abigail Edwards, Ashley D Sawle, Chandra Chilamakuri, Kamal Kishore, Stephane Ballereau, Zeynep Kalendar Atak, Hugo Tavares, Jon Price, Katarzyna Kania, Roderik Kortlever, Adam Reid, Tom Smith

Apologies if we have missed anyone!
