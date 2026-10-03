# Notas metodológicas de revisión

## 1. Unidad de análisis

El insumo DENUE contiene registros por establecimiento. Para el análisis histórico se construyeron conteos por clase SCIAN de seis dígitos y posteriormente unidades homologadas longitudinales.

## 2. Universo analizado

- Comercio al por menor: sector 46.
- Servicios: sectores 48, 49, 51, 52, 53, 54, 56, 61, 62, 71, 72 y 81.

El comercio al por mayor (43), las actividades gubernamentales (93) y la manufactura no forman parte del universo principal.

## 3. Versiones SCIAN

- 2010–2013: SCIAN 2007.
- 2015–2017: SCIAN 2013.
- 2018–2023: SCIAN 2018.
- 2024–2026: SCIAN 2023.

La comparación longitudinal no se realizó concatenando directamente códigos de versiones distintas. Se construyó un diccionario de homologación y se resolvieron correspondencias uno-a-uno, agregaciones, desagregaciones y familias complejas.

## 4. Resultado de la homologación

El diccionario final contiene 350 unidades homologadas con representación en las cuatro versiones SCIAN. El panel resultante contiene 5,600 observaciones (350 unidades × 16 cortes).

## 5. Familia FL09 e incertidumbre acotada

FL09 contiene una ambigüedad intersectorial vinculada con los códigos 811121, 811123 y 811129. Por ello, el panel conserva un intervalo mínimo–máximo. La amplitud máxima del universo total es de un establecimiento.

## 6. Discontinuidades 2019 y 2024

La clase 812110 fue auditada a nivel de establecimiento.

- 2018–2019: 1,767 → 2,328 (+561). Tras descontar tres posibles cambios de ID, quedaron 829 exclusivos del corte inicial y 1,390 exclusivos del corte final. De los exclusivos finales, 1,363 (98.06 %) tienen `fecha_alta = 2019-11`.
- 2023–2024: 2,334 → 3,128 (+794). Tras descontar un posible cambio de ID, quedaron 943 exclusivos del corte inicial y 1,737 exclusivos del corte final. De los exclusivos finales, 1,688 (97.18 %) tienen `fecha_alta = 2024-11`.

Estos resultados sustentan una interpretación cautelosa: los saltos netos no deben equipararse automáticamente con nacimientos empresariales.

## 7. Corrección documental de la familia FL03

En el inventario histórico aparece un establecimiento con código 531116 en 2022. La narrativa de la familia FL03 fue corregida para reconocer explícitamente esta observación. El dato siempre permaneció incorporado en la serie homologada y en los controles; por tanto, la corrección afecta únicamente la descripción metodológica y no modifica conteos, paneles ni resultados.

## 8. Bitácora y cuaderno reproducible

La bitácora original conserva pruebas, rutas, salidas y correcciones realizadas durante el desarrollo. El cuaderno reproducible presenta la ruta analítica depurada y ejecutable desde los insumos derivados incluidos.
