# Quail phenotypes analyses

## Objective:

Study the effects of *in-ovo* injection of treatments on quail growth and reproduction.

## Table containing phenotyping data of quails:
- 1979 individuals (male and female) from G0 generation
- 4 lines backgrounds (A, B, S+ and DD)
- 3 treatments (Genistein, 5Aza and Bisphenol) and 2 controls (injected and non-injected)
- 2 batches 
- Measured traits: growth (8,21,36,78 days) and egg-laying (egg number, age at first egg) 
 
## Library installation:

### Required libraries:

- **Figures:** *ggplot2*, *gridExtra*, *gridGraphics*, *cowplot*, *ggpubr*, *viridis*, *circlize*, *ComplexHeatmap*
- **linear mixed model:** *nlme*, *MASS*
- **Anova:** *car* 
- **Tukey HSD test:** *emmeans* 
- **Data manipulation:** *dplyr*, *tidyr*

Command examples to install a library:
**On markdown *R* script:**
```{r}
install.packages("tidyr", type = "source")
install.packages("data.table", repos="https://Rdatatable.gitlab.io/data.table")
install.packages("cdata", source="https://www.rdocumentation.org/packages/cdata")
```
```{r}
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install("limma")
```

**On terminal:**
```
sudo apt-get install r-cran-devtools
sudo apt install r-bioc-ComplexHeatmap
```
