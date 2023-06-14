# Day 3

## Runing a Seurat tutorial

1. Please log into your lab computer and create a working directory `day_3`. Alternatively you can login into https://vlab.humboldt.edu if working remotely.

2. Install the following packages and follow the tutorial

***NOTE*** when the Rstudio asks "Do you want to install from sources the package which needs compilation?" answer "NO"

```
install.packages("dplyr")
install.packages("Seurat")
install.packages("patchwork")


library(dplyr)
library(Seurat)
library(patchwork)
```

3. Create a folder called `day_3` in your Documents

4. Download the following data https://cf.10xgenomics.com/samples/cell/pbmc3k/pbmc3k_filtered_gene_bc_matrices.tar.gz to `day_3` 

5. This is a double compressed file. Decompress the file by right clicking and then selecting the options `7-zip` `Extract here`. Repeat this with the `*.tar` file

6. Set the folder where the data is as your working directory and import the data

```
setwd("YOUR_USER/Documents/day_3/pbmc3k/filtered_gene_bc_matrices/hg19/")

pbmc.data <- Read10X(data.dir = ".")
```

7. Follow the tutorial found here https://satijalab.org/seurat/articles/pbmc3k_tutorial.html Make sure that the path to the data is correct and is written using forward slashes 

