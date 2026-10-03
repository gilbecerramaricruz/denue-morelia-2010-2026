# Disponibilidad de datos

## Fuente primaria

Los datos originales proceden del Directorio Estadístico Nacional de Unidades Económicas (DENUE) del Instituto Nacional de Estadística y Geografía (INEGI).

Portal DENUE:
https://www.inegi.org.mx/app/mapa/denue/

## Datos no incluidos en el repositorio público

Para mantener este repositorio ligero y evitar redistribuir innecesariamente registros individuales completos, no se publican aquí los CSV municipales de Morelia usados en las auditorías micro de los cortes 2018, 2019, 2023 y 2024.

Esos archivos se conservan en el paquete privado de revisión de la investigación.

## Datos derivados incluidos

Sí se incluyen:

- conteos anuales por clase SCIAN;
- inventario histórico de clases;
- diccionario de 350 unidades homologadas;
- tablas de correspondencia y controles;
- panel histórico homologado;
- resultados agregados y auditorías resumidas.

## Reproducción desde datos originales

La bitácora `02_BITACORA_ORIGINAL_DENUE.ipynb` documenta el proceso seguido para descargar, inspeccionar, depurar y extraer los cortes históricos. Para una reproducción completa desde los archivos estatales originales, el investigador debe descargar las ediciones históricas correspondientes del DENUE y mantener la estructura de archivos descrita en la bitácora.
