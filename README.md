# Creación de paquetes de software de R/Bioconductor

Este es el material del mini curso "Creación de paquetes de software de R/Bioconductor" ofrecido por la Red Mexicana de Bioinformática.

Fecha: 16 de julio de 2021

Instructores: 
- [Marcel Ramos](https://cunyisph.org/team/marcel-ramos/)
- [Leonardo Collado Torres](https://lcolladotor.github.io/es/) 

## Materiales

- [Introducción a las paqueterías de Bioconductor](https://docs.google.com/presentation/d/13JZEuUCvzxH9HsBMAfXBxC7TexGfSQcaPWHu4GngU58/edit#slide=id.p)
- [biocthis: crea paquetes de Bioconductor](https://speakerdeck.com/lcolladotor/biocthis-conectar2021)

## Pre-requisitos

Para esta sesión necesitas instalar los siguientes paquetes de R:

```
if (!requireNamespace("remotes", quietly = TRUE)) {
      install.packages("remotes")
  }
 
## Paquetes de CRAN
remotes::install_cran(
    c(
        "available",
        "BiocManager",
        "devtools",
        "knitr",
        "pkgdown",
        "RefManageR",
        "rmarkdown",
        "rstudioapi",
        "sessioninfo",
        "styler",
        "usethis"
    )
)
 

## Paquetes de Bioconductor
remotes::install_cran("BiocManager")
BiocManager::version)()
# El anterior comando debe mostrar que estás usando la versión 3.13
BiocManager::install("biocthis")
BiocManager::install("BiocStyle")

```

