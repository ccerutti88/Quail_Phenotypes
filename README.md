# Quail phenotypes analyses

## Library installation:

```{r}
install.packages("tidyr", type = "source")
install.packages("data.table", repos="https://Rdatatable.gitlab.io/data.table")
install.packages("cdata", source="https://www.rdocumentation.org/packages/cdata")
```

### *devtools*:

```
sudo apt-get install r-cran-devtools
```

### *limma*, *stringr*, *rtracklayer*, *edgeR* and *ComplexHeatmap*:

On terminal...:

```
sudo apt install r-bioc-limma
```

and then on markdown R script:

```{r}
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install("limma")
```

## Objective:

To evaluate whether or not epigenetic modifications applied to animals are transmitted or not during generations and correlated to differences in phenotypic performance.

## Table containing phenotyping data of quails:

- chemical treatment applied in the egg inducing epigenetic mark modifications, affecting DNA methylation (embryos receiving this treatment or not correspond to the G0 generation)
- individuals from G1 generation
- 4 lines backgrounds: A, B, S+ and DD
- 3 treatments: Genistein, 5Aza and Bisphenol
- phenotyping data on production traits: growth, oviposition
- 100 G1 animals for each line and for each treatment, in 2 batches => 1979 individuals
 => Determine which characters are affected by the tested processing.
