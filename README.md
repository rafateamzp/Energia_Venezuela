# Sistema eléctrico de Venezuela

Repositorio de datos geográficos abiertos sobre la infraestructura del sistema eléctrico de Venezuela. Incluye una capa de líneas en formato GeoJSON y la misma clase de datos en un conjunto de archivos Shapefile.

## Contenido

- [`power_lines_VEN.geojson`](power_lines_VEN.geojson): capa GeoJSON de líneas eléctricas.
- [`240904_Energia_electrica_venezuela_WGS84/`](240904_Energia_electrica_venezuela_WGS84/): capa Shapefile, compuesta por los archivos `.shp`, `.shx`, `.dbf`, `.prj` y archivos auxiliares.

El sistema de referencia indicado para la capa Shapefile es **WGS 84 (EPSG:4326)**, con coordenadas geográficas en grados.

## Uso

### QGIS

1. Descarga o clona este repositorio.
2. Para el GeoJSON, abre `power_lines_VEN.geojson` en QGIS.
3. Para el Shapefile, abre `240904_Energia_electrica_venezuela_WGS84/240904_Energia_electrica_venezuela_WGS84.shp`. Mantén juntos los archivos que comparten el mismo nombre base para que la capa se lea correctamente.

### Python

Puedes leer el GeoJSON con GeoPandas:

```python
import geopandas as gpd

lineas = gpd.read_file("power_lines_VEN.geojson")
print(lineas.head())
print(lineas.crs)
```

Para usar el Shapefile, sustituye la ruta por:

```python
lineas = gpd.read_file(
    "240904_Energia_electrica_venezuela_WGS84/"
    "240904_Energia_electrica_venezuela_WGS84.shp"
)
```

## Notas

- El GeoJSON puede abrirse directamente en herramientas que admiten ese formato.
- Los archivos Shapefile son un conjunto: no elimines ni separes sus componentes.
- Este repositorio no especifica actualmente una licencia ni documenta la fuente original, la fecha de actualización de los datos o la definición de los atributos. Verifica esos detalles antes de reutilizar o redistribuir los datos.

## Contribuciones

Las mejoras en la documentación y las correcciones de los datos son bienvenidas mediante issues o pull requests.
