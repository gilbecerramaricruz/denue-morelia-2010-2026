# Cómo reproducir la etapa exploratoria 2013–2015

## Archivos que sí contiene esta publicación

- `06_DEMOGRAFIA_SERVICIOS_ALIMENTOS/02_LINKAGE_2013_2015_EXPLORATORIO.ipynb`: notebook ordenado para ejecutar de principio a fin; **no** contiene salidas individuales ni aceptación de enlaces.
- `DOCUMENTACION/NOTA_AVANCE_DENUE_2013_2015.md`: nota explicativa para comentarios del profesor.
- `DOCUMENTACION/RESUMEN_AUDITORIAS_DENUE_2013_2015.md`: resultados agregados y límites metodológicos.
- `DOCUMENTACION/PROTOCOLO_REVISION_DENUE_722.md`: protocolo de una revisora, todavía provisional.

## Archivos deliberadamente ausentes

No se publican los CSV maestros de establecimientos, números telefónicos, coordenadas individuales, expedientes del piloto ni el CSV con 1,146 enlaces provisionales. El notebook original de 132 celdas permanece local como **bitácora privada** porque reúne resultados individuales, pruebas antiguas y celdas dependientes de ejecución previa. Esta versión pública no declara reproducibles esas decisiones anteriores hasta contar con un pipeline independiente y validado.

## Ejecución

Requiere Python 3, `pandas`, `numpy`, `scipy` y `ipykernel`/Jupyter. Los archivos de entrada deben llamarse `DENUE_2013_MORELIA.csv` y `DENUE_2015_MORELIA.csv` y corresponder a las versiones auditadas. La forma más sencilla es tenerlos en la carpeta `DENUE_HISTORICOS/01_MORELIA_LIMPIO` junto a la carpeta del repositorio. Si están en otra ubicación, establecer la variable de entorno `DENUE_MORELIA_DIR` antes de abrir Jupyter.

Se comprobarán las huellas SHA256 de ambos CSV, sus filas, sus claves originales y su universo 722. Luego, **Kernel → Restart & Run All** produce los resúmenes agregados. Si falta la carpeta local con los enlaces preliminares, se omitirá solamente la comparación opcional con esos 1,146 pares.

No se han ejecutado estos cálculos sobre los dos CSV de Morelia dentro de esta entrega porque los datos maestros no se adjuntaron. La estructura y la sintaxis de esta versión se revisaron por separado; **los valores publicados corresponden a las salidas originales guardadas en la bitácora y compartidas durante la auditoría**, no a una nueva ejecución validada.

## Antes de publicar

Revisar `git status --short`, el contenido del notebook y el resumen. Después incorporar sólo los cinco archivos documentados, hacer `commit` y `push` desde el repositorio existente. No crear otro repositorio ni ejecutar `git init` en la carpeta de trabajo.
