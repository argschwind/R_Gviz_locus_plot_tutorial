# R Gviz locus plot tutorial

This tutorial whows how to make genomic locus plots in R using the `Gviz` and `GenomicInteractions` packages.

<div align="center">
  <img src="figures/locus_plot.png" width=95% height=95%>
</div>

The `slides.html` file contains the slides which can be viewed in a web browser (e.g. Chrome of Safari). All code for the tutorial is in `slides.Rmd`,
which can be used to reproduce the shown plots and as basis try making your own plots.

## Executing the code

To follow along the tutorial, the following R packages have to be installed:

```{r}
# make sure Bioconductor installer is installed
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

# install Bioconductor packages
BiocManager::install("Gviz")
BiocManager::install("GenomicInteractions")
BiocManager::install("rtacklayer")

# install packages from CRAN
install.packages("dplyr")
install.packages("data.table")
```

## Further reading

The [Gviz User Guide](https://bioconductor.org/packages/release/bioc/vignettes/Gviz/inst/doc/Gviz.html) provides a very nive overview of possible plots
that can be made. More information on the `GenomicInteractions` package can be found on
[Bioconductor](https://bioconductor.org/packages/release/bioc/html/GenomicInteractions.html).
