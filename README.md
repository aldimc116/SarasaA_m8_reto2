# Proyecto de Ciencia de Datos Reproducible: Salud y Felicidad Autopercibidas en Europa

Autoría: Alba Sarasa

**Licencia:** Todos los materiales originales de este repositorio se pueden copiar, modificar, distribuir y utilizar estos materiales sin restricción alguna.

Este proyecto forma parte de un trabajo académico de Ciencia de Datos Reproducible.\
El objetivo principal es analizar la relación entre **salud** y **felicidad autopercibidas** en distintos países europeos, así como su variación según la edad, género y situación de inmigración en el país (nativo/no nativo).

------------------------------------------------------------------------

## 📂 Contenidos del repositorio

-   `/Data` → Carpeta con los datos utilizados (European Social Survey, ESS).

    -   `ESS11-subset.csv` → Base de datos obtenida de la web oficial de [ESS](https://www.europeansocialsurvey.org/).

    -   `DataDepuration.Rmd` → Código en **Rmarkdown** para la depuración de la base de datos

    -   `ESS11-depurado.csv` → Base de datos depurada. Se obtiene ejecutando `DataDepuration.Rmd`

-   `/Dashboard` → Carpeta con el código para crear el dashboard del proyecto y el archivo .html que se obtiene.

    -   `DashboardCode.Rmd` → Código en **Rmarkdown** para la creación del Dashboard

    -   `DashboardCode.html` → Dashboard. Se obtiene ejecutando `DashboardCode.Rmd`

-   `/Report` → Carpeta con el código para crear el informe del proyecto y el archivo .html que se obtiene.

    -   `ReportCode.Rmd` → Código en **Rmarkdown** para obtener el informe técnico del proyecto.

    -   `ReportCode.html` → Informe técnico en formato .html que resume los hallazgos principales del proyecto. Se obtiene ejecutando `ReportCode.Rmd`

-   `/Presentation` → Carpeta con el código para crear la presentación del proyecto y el archivo .html que se obtiene.

    -   `PresentationCode.Rmd` → Código en **Rmarkdown** para obtener la presentación del

    -   `PresentationCode.html` → Presentación en **html** con los principales hallazgos y gráficos sintetizados.

------------------------------------------------------------------------

## 🛠️ Herramientos utilizadas

-   **R** studio:
    -   `> R.version _platform x86_64-apple-darwin20arch x86_64os darwin20system x86_64, darwin20statusmajor 4minor 4.2year 2024month 10day 31svn rev 87279language Rversion.string R version 4.4.2 (2024-10-31) nickname Pile of Leaves`
-   Paquetes necesarios:
    -   `c( "knitr", "ggplot2", "dplyr", "ggridges", "viridis", "readr", "here", "scales", "patchwork", "tidyr", "gt", "flexdashboard", "plotly", "shiny", "sf", "rnaturalearth")`

------------------------------------------------------------------------

## 🚀 Instrucciones de uso

1.  Clonar el repositorio:

    ``` bash
    git clone https://github.com/usuario/proyecto-salud-felicidad.git
    ```

2.  Abrir RStudio.\

3.  Cargar los datos del ESS en la carpeta `Data/`.\

4.  Ejecutar e archivo `DataDepuration.Rmd`

5.  Renderizar los documentos:

    ``` r
    rmarkdown::render("DashboardCode.Rmd")
    rmarkdown::render("ReportCode.Rmd")
    rmarkdown::render("PresentationCode.Rmd")
    ```

Los resultados aparecerán en la carpeta correspondiente.
