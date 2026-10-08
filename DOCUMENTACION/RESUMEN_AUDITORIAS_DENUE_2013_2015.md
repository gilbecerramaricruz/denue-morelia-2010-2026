# Avances y auditorías de vinculación DENUE 2013–2015

**Subsector SCIAN 722, servicios de preparación de alimentos y bebidas, municipio de Morelia.**  
*Resultados de exploración, 7 de octubre de 2026. Ningún enlace se considera validado en este documento.*

## Qué se revisó

Estoy reconstruyendo correspondencias entre los registros de establecimientos de los cortes 2013 y 2015 del DENUE. El trabajo no consiste en comparar únicamente el número de establecimientos; la primera tarea es determinar si dos registros de distintas ediciones podrían representar la misma unidad.

Se verificaron **4,239 establecimientos en 2013** y **5,376 establecimientos en 2015**, ambos del subsector 722. Los identificadores originales entre estos cortes no proporcionan continuidad directa para las unidades de este universo. Por esa razón, las coincidencias se buscaron provisionalmente con nombre, teléfono, domicilio y ubicación, conservando las claves SCIAN originales.

## Qué se hizo primero

Se recuperaron **1,146 parejas provisionales**, integradas por 612 coincidencias aceptadas por nombres únicos, 164 por nombres repetidos, 185 por teléfono, 180 por una etapa geográfica y cinco por una segunda ronda. En esta clasificación original, **812 se consideraron «respaldadas» y 334 «probables»**. Una auditoría comprobó que las 1,146 parejas utilizaban índices originales válidos del subsector 722, sin reutilizar registros de 2013 ni de 2015. **Esta integridad uno-a-uno no valida las identidades.**

Los restantes **3,093 registros de 2013** y **4,230 registros de 2015** no tenían enlace aceptado en ese esquema. Esto **no equivale a 3,093 cierres ni a 4,230 nacimientos**.

## Qué me hizo replantear el procedimiento

- **Nombres genéricos.** En ambas ediciones hay nombres como «COCINA ECONÓMICA» o «TAQUERÍA». Al estandarizar, un mismo nombre genérico produce muchas combinaciones que no distinguen establecimientos.
- **Teléfonos no siempre exclusivos.** De los **461 pares** con teléfono coincidente entre 722, **418 tenían ese número asociado a un único registro en cada corte de todo Morelia**; los otros **43 pares** compartían número con otros registros en al menos un corte. De los 185 enlaces antes aceptados por teléfono, **ocho tenían teléfono compartido**. Ser exclusivo es apoyo, no prueba de identidad.
- **Domicilio y coordenadas no siempre coinciden.** Entre los 1,146 pares provisionales, **267 tenían coordenadas separadas por más de 25 metros**; dentro de esos 267, **128 conservaban calle y número exterior iguales**. No se debe imponer una frontera espacial rígida ni concluir automáticamente que hay mudanza.
- **Concentraciones de establecimientos.** En Nicolás Bravo #304, 25 registros de 2013 compartían el mismo punto geográfico. Por tanto, contar vecinos próximos no equivale a contar competidores de identidad.
- **Información ausente.** En 2013, 1,238 de 4,239 establecimientos del subsector (29.21%) tenían teléfono normalizado; en 2015 fueron 1,550 de 5,376 (28.83%). La razón social estaba disponible para 201 establecimientos en 2013 (4.74%) y 211 en 2015 (3.92%). Si falta un teléfono o razón social, la comparación es indeterminada, no un desacuerdo.
- **Actualizaciones del directorio.** La concentración de fechas de incorporación exige tratarlas como dato administrativo y no como fecha de nacimiento empresarial.

## Búsqueda más amplia: candidatos, no coincidencias confirmadas

Se construyó una generación multirruta de candidatos sin aceptar automáticamente parejas. Se recuperaron **162,512 pares candidatos** con cinco rutas: nombre exacto (**3,077**), nombre base sin el sufijo «SIN NOMBRE» (**38,337**), teléfono (**461**), domicilio de calle+número (**4,109**) y geografía dentro de 250 metros (**125,616**). El total es menor que la suma de las rutas porque varios pares aparecieron por más de una.

De los **162,512 pares candidatos**, **157,501 (96.92%)** se recuperaron mediante una sola familia de información; **120,612** se recuperaron solamente por geografía y **36,852**, solamente por nombre. La nueva búsqueda recuperó las **1,146 parejas provisionales**, pero esta comprobación no demuestra que sean verdaderas.

Quedaron **15 establecimientos de 2013** y **164 de 2015** sin candidatos mediante esas rutas dentro del subsector 722. La búsqueda fuera del subsector y las rutas adicionales son tareas pendientes; esos registros no deben clasificarse como cierres o nacimientos.

## Revisión y validación: estado real

Se preparó un **piloto de 55 expedientes**, que reúne **1,427 pares candidatos**. Las fichas de referencia y candidatos están completas, pero todavía **no se cuenta con los 55 dictámenes manuales concluidos**, ni se han estimado precisión ni exhaustividad del algoritmo. La revisión principal la realizará una sola investigadora; no se afirmará una validación entre dos revisores independientes.

Los expedientes P001 y P002 se discutieron como ejemplos de desarrollo del protocolo, por lo que no se considerarán una evaluación ciega. Las decisiones anteriores, incluidos los 1,146 enlaces, siguen siendo provisionales.

## Qué se propone y qué no se ha hecho

Se propone combinar reglas multivariables con una puntuación de evidencia calibrada, resolver conflictos uno-a-uno sin forzar coincidencias, mantener casos ambiguos y validar la precisión y las correspondencias omitidas con una muestra independiente. **Aún no se han calibrado pesos probabilísticos, no se ha ejecutado la asignación final y no hay estimaciones de supervivencia empresarial.**

El notebook público reproduce la preparación de maestros, la generación de candidatos y las comparaciones agregadas; las decisiones y expedientes individuales se conservan fuera del repositorio.
