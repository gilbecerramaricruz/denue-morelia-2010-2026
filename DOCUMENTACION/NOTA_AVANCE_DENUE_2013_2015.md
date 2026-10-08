# Nota de avance y consulta metodológica

**Comparación DENUE 2013–2015 | Establecimientos de servicios de preparación de alimentos y bebidas (SCIAN 722), Morelia**

*Documento de trabajo para comentarios del profesor. 7 de octubre de 2026.*

**Estado del trabajo:** los enlaces entre establecimientos siguen siendo provisionales; esta nota plantea una forma de validarlos.

## Cómo llegué a esta duda

Estoy trabajando con 16 cortes históricos del DENUE, de 2010 a 2026, para estudiar cómo cambian los establecimientos de servicios de preparación de alimentos y bebidas (SCIAN 722) en Morelia. Al principio parecía suficiente comparar cuántos negocios había en cada año, pero me di cuenta de que, para estudiar su permanencia, primero necesito saber si un registro de un año corresponde al mismo establecimiento en el siguiente.

Decidí comenzar por la comparación de 2013 y 2015. En 2013 encontré 4,239 establecimientos del subsector 722 y en 2015, 5,376. El problema es que los identificadores de esos dos cortes no permiten seguir directamente a los mismos negocios. Además, cambiaron algunas claves SCIAN y hubo actualizaciones del directorio. También vi que la fecha de incorporación se repite en miles de registros, por lo que no la estoy tomando como fecha de apertura. Por eso no sería correcto tomar cada registro nuevo como un negocio que nació, ni cada registro que deja de aparecer como uno que cerró.

## Qué he trabajado hasta ahora

Primero busqué coincidencias mediante nombres, teléfonos, domicilios y ubicación geográfica. Fui revisando los casos donde varios negocios tenían nombres parecidos, donde un teléfono podía corresponder a más de un establecimiento o donde las coordenadas no coincidían del todo. Así obtuve 1,146 parejas provisionales: 812 clasificadas inicialmente como respaldadas y 334 como probables. También comprobé que ningún registro de 2013 ni de 2015 se hubiera utilizado dos veces.

Después hice una búsqueda más amplia para no quedarme solamente con las coincidencias que ya había encontrado. Esta revisión produjo 162,512 parejas posibles entre los establecimientos de ambos años. Eso no significa que existan tantos negocios relacionados: son opciones que el procedimiento debe comparar y descartar o dejar pendientes. De hecho, recuperó las 1,146 parejas iniciales, pero eso tampoco demuestra que todas sean correctas.

Lo que más me hizo dudar fueron los nombres genéricos, como “COCINA ECONÓMICA” o “TAQUERÍA”; los teléfonos que se comparten; y las coordenadas que cambian incluso cuando el domicilio escrito es el mismo. También encontré casos donde un teléfono apunta a un negocio y la ubicación parece apuntar a otro. Si acepto enlaces solo porque coinciden en una variable, corro el riesgo de inventar una permanencia que quizá no existió.

Por eso preparé un primer grupo de 55 expedientes para revisar con mayor detalle, que reúne 1,427 parejas candidatas. Es una prueba para afinar los criterios de revisión, no una muestra con la que ya pueda afirmar qué tan preciso es el procedimiento. De momento, los 1,146 enlaces siguen siendo provisionales.

## Cómo propongo continuar

Mi idea es dejar de aceptar coincidencias por etapas aisladas y revisar cada pareja considerando varias evidencias al mismo tiempo: nombre, teléfono, domicilio, coordenadas y actividad registrada, sin olvidar cuándo faltan datos o existen otros candidatos. También quiero que un establecimiento no pueda quedar vinculado automáticamente con dos del corte siguiente, y que los casos dudosos permanezcan sin resolver hasta tener evidencia suficiente.

Estoy considerando combinar reglas claras de coincidencia con un método estadístico de vinculación, pero no quiero poner porcentajes de confianza o pesos sin antes comprobar que funcionan con estos datos. Una vez definido el procedimiento, haría una revisión manual con criterios escritos y después usaría una muestra nueva, separada del desarrollo, para estimar los errores. Esa revisión la realizaría yo, de modo que señalaría expresamente que no se trata de una evaluación entre dos revisores independientes.

Solo después de resolver qué registros probablemente representan el mismo establecimiento pasaría al análisis demográfico: cuáles aparecen en varios cortes, cuáles dejan de observarse y cuáles reaparecen. Los posibles nacimientos, cierres o tiempos de supervivencia requerirían una justificación adicional; no se deducirían automáticamente de una diferencia entre directorios.

## Lo que quisiera consultarle

Antes de aplicar este procedimiento al resto de los años, me gustaría conocer su opinión sobre tres puntos: si le parece adecuada esta forma de reconstruir la identidad de los establecimientos; si considera conveniente combinar varios criterios de comparación dejando los casos ambiguos sin enlace; y si la revisión manual y la muestra posterior para medir errores son suficientes para sustentar la metodología, considerando que la revisión la haría yo.

Mi intención es dejar definida una forma de trabajo que pueda repetirse en los demás cortes y documentarse en GitHub. Prefiero revisar ahora estas decisiones, en lugar de avanzar con resultados que después no pueda defender metodológicamente.

## Fuentes de apoyo

- Instituto Nacional de Estadística y Geografía (INEGI). (2021). Directorio Estadístico Nacional de Unidades Económicas: metadatos de actualización e incorporación de unidades económicas. https://www.inegi.org.mx/rnm/index.php/catalog/668

- Fellegi, I. P., y Sunter, A. B. (1969). A theory for record linkage. Journal of the American Statistical Association, 64(328), 1183–1210. https://doi.org/10.1080/01621459.1969.10501049

- Office for National Statistics (ONS). (2021). Developing standard tools for data linkage: February 2021. https://www.ons.gov.uk/methodology/methodologicalpublications/generalmethodology/onsworkingpaperseries/developingstandardtoolsfordatalinkagefebruary2021
