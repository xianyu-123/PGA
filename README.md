# PGA
This is an alternative installation method for BiocManager::install("wenbostar/PGA"). 

Orign: https://github.com/wenbostar/PGA


```
download wenbostar-PGA-v1.9.1-86-ga0d6866.tar.gz from https://drive.google.com/file/d/13gnP1v7NDkSrz5ZaPZfU3_3m5M1hKNlp/view?usp=sharing

conda install conda-forge::r-base=4.4.3
conda install -c conda-forge r-curl
conda install bz1::libgcc-ng
conda install -c conda-forge zlib
conda install -y -c conda-forge r-stringi
conda install xz
conda install -c conda-forge libxml2
conda install conda-forge::expat

options(BioC_mirror="https://mirrors.westlake.edu.cn/bioconductor")

install.packages("remotes")
remotes::install_version("data.table", version = "1.15.2")
install.packages("Matrix")
remotes::install_github('bioconductor-source/rTANDEM')
install.packages(c("ggplot2", "pheatmap", "processx", "readr", "seqinr"))

if (!requireNamespace("BiocManager", quietly = TRUE))
install.packages("BiocManager")

BiocManager::install(c("IRanges", "GenomicRanges", "Biostrings", "S4Vectors",
"Rsamtools", "GenomicFeatures", "biomaRt",
"VariantAnnotation", "rtracklayer", "customProDB","rTANDEM", "Nozzle.R1"))

install.packages('wenbostar-PGA-v1.9.1-86-ga0d6866.tar.gz')

