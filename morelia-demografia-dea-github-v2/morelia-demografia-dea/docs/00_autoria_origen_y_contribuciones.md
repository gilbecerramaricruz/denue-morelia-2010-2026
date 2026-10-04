# Autoría, origen de la idea y contribuciones

## 1. Origen intelectual del proyecto

La idea central de este proyecto fue planteada por **Antonio Kido Cruz**.

El concepto no surgió de una generación automática de software ni de una propuesta autónoma de inteligencia artificial. La secuencia intelectual fue definida por el investigador:

1. estudiar primero la **demografía de los negocios** en Morelia;
2. identificar qué tipos de establecimientos nacen, sobreviven o desaparecen;
3. analizar esas diferencias por giro, tamaño, zona y periodo;
4. usar esa evidencia para formar grupos de establecimientos suficientemente homogéneos;
5. aplicar posteriormente **Análisis Envolvente de Datos (DEA)** para identificar eficiencia relativa, peers y slacks;
6. diseñar rutas de intervención para los establecimientos menos eficientes;
7. contrastar después los resultados con empresas reales, idealmente con apoyo de **CANACO Morelia**.

También fue planteado por Antonio Kido Cruz que el análisis no debía concentrarse únicamente en los estratos con mayor número de establecimientos. Un grupo pequeño, por ejemplo negocios de 51 o más trabajadores, puede ser empíricamente relevante si presenta una mortalidad elevada. Por ello, la demografía debe estimarse para todos los tamaños disponibles antes de seleccionar las DMU para DEA.

La formulación de preguntas como las siguientes corresponde al razonamiento sustantivo del proyecto:

- ¿Un restaurante abierto en Morelia tiene menor supervivencia que una tienda de abarrotes?
- ¿Los negocios de 0–5 trabajadores desaparecen más rápidamente que los de 6–10?
- ¿Existen zonas de Morelia donde sistemáticamente mueren más negocios?
- ¿Qué giros muestran simultáneamente mucha creación y mucha mortalidad?
- ¿La pandemia modificó de manera permanente la función de supervivencia de determinados giros?
- ¿Qué establecimientos son comparables tecnológicamente para un análisis DEA?
- ¿Qué slacks explican la ineficiencia de los negocios menos eficientes?
- ¿Qué tipo de intervención es razonable y en qué casos DEA no debe utilizarse como herramienta de recomendación?

## 2. Papel del conocimiento humano y de la literatura previa

El proyecto se apoya en conceptos desarrollados previamente por investigadores, instituciones estadísticas y especialistas humanos.

La **demografía de negocios** emplea ideas de nacimiento, supervivencia, muerte, cohorte, riesgo y esperanza de vida empresarial. Estas metodologías han sido desarrolladas por organismos estadísticos y literatura especializada y, en México, han sido aplicadas por el **INEGI**.

El **Análisis Envolvente de Datos (DEA)** es una metodología desarrollada en la literatura académica para estudiar eficiencia relativa entre unidades de decisión comparables. Conceptos como frontera eficiente, peers, slacks, rendimientos a escala y supereficiencia provienen de esa tradición científica.

Por tanto, el proyecto combina tres niveles de aportación humana:

- conocimiento acumulado de la literatura científica;
- información estadística generada por instituciones como INEGI;
- diseño específico del problema de investigación propuesto por Antonio Kido Cruz para Morelia.

## 3. Papel específico de ChatGPT en este proyecto

ChatGPT ha funcionado como una **herramienta de apoyo técnico, metodológico y computacional**, bajo las decisiones sustantivas del investigador.

Sus tareas principales han sido:

### 3.1 Tratamiento de bases extensas

Se procesaron archivos masivos del DENUE correspondientes al sector 72.

Para la edición 2026 se trabajó con:

- `denue_00_72_1_csv.zip`
- `denue_00_72_2_csv.zip`

A partir de estos archivos se:

- descomprimieron y leyeron los CSV;
- filtraron registros por entidad federativa;
- filtraron registros por municipio;
- filtraron establecimientos por clase SCIAN;
- se identificaron los registros correspondientes a **SCIAN 722511** en Morelia;
- se verificó que el resultado contuviera **750 establecimientos**, consistente con el panel agregado previamente construido;
- se conservaron identificadores como ID DENUE y CLEE;
- se organizaron variables de ubicación, actividad, tamaño, AGEB, manzana, coordenadas y fecha de alta;
- se normalizaron nombres de establecimientos para detectar posibles repeticiones o cadenas;
- se construyeron variables auxiliares para clasificación de grupos comparables;
- se generaron archivos Excel de trabajo y una estructura de repositorio reproducible.

### 3.2 Estructuración metodológica

ChatGPT ayudó a transformar la idea original en una arquitectura reproducible:

- demografía empresarial;
- análisis por tamaño;
- análisis territorial;
- comparación entre giros;
- análisis del efecto pandemia;
- formación posterior de DMU;
- DEA;
- slacks;
- intervención.

### 3.3 Programación y documentación

ChatGPT preparó:

- scripts iniciales en R;
- archivos de configuración;
- estructura de carpetas;
- documentación metodológica;
- plantillas para panel longitudinal;
- archivos Excel procesados;
- criterios para identificar grupos potencialmente comparables.

## 4. Lo que ChatGPT no decidió

ChatGPT no debe considerarse autor intelectual autónomo del proyecto.

No decidió por sí solo:

- estudiar Morelia;
- usar supervivencia empresarial como primera etapa;
- combinar demografía de negocios con DEA;
- usar los slacks como base para intervención;
- llevar posteriormente el enfoque a CANACO Morelia;
- no excluir estratos pequeños;
- distinguir entre negocios intervenibles y negocios cuyo problema puede ser estructural;
- formular la estrategia global de investigación.

Esas decisiones derivan del planteamiento del investigador y de la discusión metodológica humana.

## 5. Responsabilidad académica

La interpretación final de resultados, la selección de variables, las decisiones metodológicas, la validación empírica y las conclusiones científicas corresponden a los autores humanos.

Los productos generados con apoyo de ChatGPT deben ser:

- revisados;
- verificados;
- contrastados con las fuentes originales;
- documentados;
- reproducibles.

El uso de inteligencia artificial no sustituye la responsabilidad científica de los autores.

## 6. Declaración sugerida de uso de inteligencia artificial

> Durante el desarrollo del proyecto se utilizó ChatGPT, de OpenAI, como herramienta de apoyo para tareas de programación, organización de bases extensas, generación de estructuras de documentación y asistencia metodológica. La concepción del problema de investigación, las preguntas, la estrategia empírica, la selección de metodologías, la interpretación de resultados y las conclusiones corresponden a los autores. Los resultados producidos mediante asistencia computacional fueron revisados y validados por los investigadores.

## 7. Aporte distintivo del proyecto

El aporte principal no consiste solamente en calcular eficiencia DEA ni en reproducir indicadores de supervivencia.

La propuesta consiste en integrar:

**demografía empresarial → selección de grupos homogéneos → DEA → slacks → intervención → validación con negocios reales**

Esa secuencia permite separar dos problemas diferentes:

- el **riesgo de desaparición** de un negocio;
- la **ineficiencia relativa** de un negocio.

Un establecimiento puede ser eficiente y pertenecer a un entorno de alta mortalidad, o puede ser ineficiente y operar en un entorno relativamente favorable. Mantener separadas ambas dimensiones es central para el diseño de intervenciones útiles.
