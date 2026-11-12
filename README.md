# Datos geográficos del sistema eléctrico de Venezuela

Este repositorio resguarda datos geográficos relacionados con el sistema eléctrico de Venezuela. Su objetivo actual es conservar y poner a disposición los archivos recibidos en sus formatos originales, sin transformaciones ni análisis adicionales.

## Fuentes y archivos

- [`power_lines_VEN.geojson`](power_lines_VEN.geojson): datos extraídos de [Overpass Turbo](https://overpass-turbo.eu/).
- [`240904_Energia_electrica_venezuela_WGS84/`](240904_Energia_electrica_venezuela_WGS84/): archivo Shapefile y componentes asociados, extraídos del [Geoportal Provita](https://geoportal.provita.org.ve/).

El archivo `.prj` del Shapefile indica el sistema de coordenadas geográficas WGS 84. Para utilizar esta capa, mantén juntos los archivos que comparten el mismo nombre base.

## Conservación y uso

Los datos se mantienen en sus formatos originales para facilitar su consulta en herramientas compatibles con información geográfica, como QGIS y bibliotecas de análisis geoespacial.

La atribución de las fuentes se incluye con fines de referencia. Este repositorio no especifica una licencia propia ni confirma las condiciones de reutilización de cada fuente. Antes de redistribuir o utilizar los datos, consulta los términos y condiciones aplicables en [Overpass Turbo](https://overpass-turbo.eu/) y el [Geoportal Provita](https://geoportal.provita.org.ve/).
