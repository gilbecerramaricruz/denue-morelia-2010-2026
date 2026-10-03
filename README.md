# Reconstrucción histórica y homologación longitudinal del DENUE de Morelia (2010–2026)

**Autora:** Maricruz Evelyn Gil Becerra  
**Programa:** Doctorado en Administración  
**Fuente principal:** Directorio Estadístico Nacional de Unidades Económicas (DENUE), INEGI.

## Objetivo

Este repositorio documenta un procedimiento reproducible para reconstruir y homologar longitudinalmente establecimientos de comercio y servicios de Morelia, Michoacán, a partir de distintas ediciones históricas del DENUE entre 2010 y 2026.

El análisis trabaja con clases SCIAN de seis dígitos y controla cambios entre las versiones SCIAN 2007, 2013, 2018 y 2023. El resultado es un panel de 350 unidades homologadas comparables en 16 cortes temporales.

## Resultados reproducibles

El notebook `01_ANALISIS_REPRODUCIBLE_DENUE_MORELIA.ipynb` permite reconstruir y verificar:

- 6,435 registros año–clase SCIAN en el inventario histórico.
- 350 unidades homologadas con cobertura en las cuatro versiones SCIAN.
- 5,600 observaciones en el panel final (350 × 16 cortes).
- Conservación de totales en los 16 cortes.
- Serie histórica general 2010–2026.
- Comparación de comercio al por menor y servicios.
- Desagregación sectorial de servicios.
- Auditorías específicas de discontinuidades en 2019 y 2024.

## Corrección documentada de FL03

La clase SCIAN `531116` forma parte de la familia homologada FL03. La auditoría identificó una observación de esta clase en 2022. La narrativa metodológica fue corregida para reflejar este hallazgo sin modificar los datos ni la homologación.

## Estructura

- `01_ANALISIS_REPRODUCIBLE_DENUE_MORELIA.ipynb`: análisis limpio y reejecutable.
- `01_ANALISIS_REPRODUCIBLE_DENUE_MORELIA.html`: versión de lectura.
- `02_BITACORA_ORIGINAL_DENUE.ipynb`: bitácora completa del procesamiento y decisiones.
- `02_CONTEOS_SCIAN/`: conteos anuales por clase SCIAN.
- `03_HOMOLOGACION_SCIAN/`: diccionarios, correspondencias y controles de homologación.
- `05_RESULTADOS/`: panel, series, tablas y controles finales.
- `DOCUMENTACION/`: notas metodológicas, disponibilidad de datos y guía de reproducción.
- `CITATION.cff`: metadatos de citación del software.

## Datos a nivel establecimiento

Los CSV municipales a nivel establecimiento usados para las auditorías micro de 2018, 2019, 2023 y 2024 **no se incluyen en este repositorio público**. Se mantienen en el paquete privado de revisión y pueden reconstruirse a partir de las ediciones históricas correspondientes del DENUE.

Esta separación mantiene el repositorio de código ligero y evita redistribuir innecesariamente archivos completos de registros individuales.

## Reproducción

1. Crear un entorno de Python.
2. Instalar las dependencias de `requirements.txt`.
3. Abrir `01_ANALISIS_REPRODUCIBLE_DENUE_MORELIA.ipynb`.
4. Ejecutar todas las celdas.
5. Revisar los controles finales.

Para las auditorías micro a nivel establecimiento, consulte `DOCUMENTACION/DISPONIBILIDAD_DE_DATOS.md`.

## Principios metodológicos

- Una aparición en DENUE no se interpreta automáticamente como nacimiento empresarial.
- Una ausencia no se interpreta automáticamente como muerte empresarial.
- `fecha_alta` se interpreta como fecha de incorporación registrada en DENUE, no como fecha de nacimiento del negocio.
- Los cortes de 2019 y 2024 se tratan como discontinuidades que requieren auditoría específica.
- La clase SCIAN de seis dígitos es el máximo nivel de desagregación usado.

## Software

El cuaderno original fue trabajado en Jupyter Notebook dentro de Antigravity y ejecutado con Python 3.11.9. El análisis utiliza principalmente pandas, NumPy y Matplotlib.

## Citación

Los metadatos de citación se encuentran en `CITATION.cff`.

## Estado de validación

El notebook reproducible fue ejecutado de principio a fin durante la preparación del paquete. Los controles finales reportaron resultados consistentes con el panel y las tablas de control entregadas.
