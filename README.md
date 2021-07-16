# Creación de paquetes de software de R/Bioconductor

Este es el material del mini curso "Creación de paquetes de software de R/Bioconductor" ofrecido por la Red Mexicana de Bioinformática.

Fecha: 16 de julio de 2021

Instructores: 
- [Marcel Ramos](https://cunyisph.org/team/marcel-ramos/)
- [Leonardo Collado Torres](https://lcolladotor.github.io/es/) 


Para descargar este material puedes dar click en el botón **Code** y selecciona la opción **Download zip**. Si lo prefieres, puedes clonar el repositorio en tu computadora usando git clone desde tu terminal.

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

