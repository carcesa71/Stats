# Guía de Estudio: Conceptos Básicos de Estadística

## 1. Significado de Estadística

La palabra "Estadística" tiene varias acepciones (significados) según el contexto:

- **Estadística como disciplina científica**: es la ciencia que se encarga de recolectar, organizar, presentar, analizar e interpretar datos, con el fin de tomar decisiones o llegar a conclusiones válidas ante la presencia de incertidumbre.
- **Estadística como conjunto de datos**: se usa coloquialmente para referirse a un conjunto de cifras o resultados numéricos sobre un tema (ej.: "las estadísticas de desempleo").
- **Estadística como medida resumen**: un valor calculado a partir de una muestra (por ejemplo, un promedio o una proporción muestral) que resume una característica.
- **División de la disciplina**:
  - *Estadística Descriptiva*: organiza, resume y presenta datos (tablas, gráficos, medidas de tendencia central y dispersión), sin generalizar más allá de los datos observados.
  - *Estadística Inferencial*: utiliza los datos de una muestra para hacer generalizaciones, estimaciones o pruebas sobre una población, incorporando el cálculo de probabilidades.

### Dato estadístico
Es el resultado de observar o medir una característica en una unidad estadística. Es la materia prima de la estadística: puede ser numérico (cuantitativo) o categórico (cualitativo), y por sí solo, antes de ser procesado, no tiene mayor utilidad; adquiere valor cuando se organiza y analiza.

---

## 2. Elementos básicos en un estudio estadístico

Al enfrentar un caso particular, es fundamental identificar correctamente estos elementos:

| Elemento | Definición |
|---|---|
| **Unidad estadística** | Cada uno de los elementos (personas, objetos, eventos) sobre los que se recolecta información. Es el "objeto" de estudio individual. |
| **Unidad de muestreo** | El elemento (o conjunto de elementos) que se selecciona en el proceso de muestreo. Puede coincidir con la unidad estadística o ser un conglomerado de ellas (ej.: si la unidad estadística es "estudiante", la unidad de muestreo podría ser "el aula" que agrupa varios estudiantes). |
| **Informante** | La persona (o fuente) que proporciona la información sobre la unidad estadística. Puede ser la misma unidad estadística (autoinformante) o un tercero (ej.: un padre que responde por su hijo). |
| **Población** | El conjunto total de unidades estadísticas que interesa estudiar y sobre las cuales se desea obtener conclusiones. |
| **Muestra** | Un subconjunto representativo de la población, seleccionado para estudiarlo y generalizar los resultados a toda la población. |
| **Característica** | El atributo, cualidad o propiedad de la unidad estadística que interesa estudiar (ej.: estado civil, ingreso, altura). |
| **Variable** | La forma operacional/medible de una característica; es lo que realmente varía de una unidad a otra y puede tomar distintos valores. |
| **Observación** | El valor específico que toma una variable en una unidad estadística determinada. |
| **Escalas de medición** | La forma en que se clasifican o cuantifican los valores de una variable. Se dividen en:<br>• **Nominal**: categorías sin orden (ej.: sexo, religión, color de ojos).<br>• **Ordinal**: categorías con orden o jerarquía, pero sin distancias exactas entre ellas (ej.: nivel educativo, satisfacción: bajo/medio/alto).<br>• **Intervalo**: valores numéricos con distancias iguales entre sí, pero sin un cero absoluto (ej.: temperatura en °C).<br>• **Razón (o de razón)**: valores numéricos con distancias iguales y un cero absoluto real, que permite hacer razones/cocientes (ej.: peso, ingreso, edad). |

---

## 3. Enumeración total vs. estudio por muestreo

| Aspecto | Enumeración total (Censo) | Estudio por muestreo |
|---|---|---|
| **Definición** | Se recolecta información de **todas** las unidades de la población. | Se recolecta información de solo una **parte** (muestra) de la población. |
| **Costo** | Generalmente más alto. | Generalmente más bajo. |
| **Tiempo** | Requiere más tiempo. | Requiere menos tiempo. |
| **Errores** | No hay error de muestreo, pero pueden existir errores no muestrales (más difíciles de controlar por el volumen de datos). | Existe error de muestreo, pero suele ser más manejable y controlable, y con frecuencia genera datos de mayor calidad por permitir mayor supervisión. |
| **Aplicación** | Útil cuando la población es pequeña o se requiere información de cada unidad individual (ej.: Censo Nacional de Población). | Útil cuando la población es grande, y basta con generalizar resultados con un margen de error conocido. |

---

## 4. Fuentes de información

- **Fuente primaria**: es aquella en la que el investigador recolecta los datos directamente de las unidades estadísticas, para el propósito específico del estudio (ej.: aplicar una encuesta propia).
- **Fuente secundaria**: es aquella en la que los datos ya fueron recolectados previamente por otra persona o institución, con otro propósito, y el investigador los reutiliza (ej.: datos del INEC, registros administrativos de otra entidad).
- **Fuente propia**: son los datos generados internamente por la misma organización o investigador a partir de sus propios registros o actividades (ej.: registros de ventas de una empresa, expedientes internos).

---

## 5. Técnicas de recolección de información no existente

Cuando la información no existe previamente (no hay fuente secundaria disponible), debe recolectarse mediante alguna de estas técnicas:

- **Observación**: el investigador registra directamente el comportamiento, hecho o fenómeno, sin necesidad de preguntar al informante (ej.: contar vehículos que pasan por una intersección).
- **Entrevista personal**: un encuestador interactúa cara a cara con el informante, formulando las preguntas del cuestionario y registrando las respuestas. Permite aclarar dudas y suele tener alta tasa de respuesta, pero es costosa y consume tiempo.
- **Entrevista telefónica**: similar a la personal, pero realizada por teléfono. Es más rápida y económica, aunque puede tener menor tasa de respuesta y limitaciones en la extensión del cuestionario.
- **Correo (cuestionario por correo)**: el cuestionario se envía al informante (físico o electrónico) para que lo complete y lo devuelva. Es económico y permite llegar a zonas dispersas, pero suele tener baja tasa de respuesta y no hay control sobre quién responde.
- **Registro**: se obtiene la información de documentos, formularios o bases de datos administrativas que ya existen como parte de un proceso rutinario (ej.: registros hospitalarios, actas de nacimiento).
- **Mixto**: combina dos o más de las técnicas anteriores, buscando aprovechar las ventajas de cada una y compensar sus limitaciones.

### Cuestionario
Es el instrumento (formulario) que contiene el conjunto ordenado y estructurado de preguntas diseñadas para obtener la información deseada de los informantes, sea de forma directa (entrevista) o auto-administrada (correo).

---

## 6. Tipos de muestras y tipos de error

### Muestras aleatorias (probabilísticas)
Son aquellas en las que **cada unidad de la población tiene una probabilidad conocida y distinta de cero de ser seleccionada**. Se basan en el azar y permiten calcular el error de muestreo y hacer inferencia estadística válida (ej.: muestreo aleatorio simple, estratificado, por conglomerados, sistemático).

### Muestras no aleatorias (no probabilísticas)
Son aquellas en las que la selección de las unidades **no se basa en el azar**, sino en criterios del investigador, la conveniencia o la disponibilidad de los sujetos. No se puede calcular el error de muestreo de forma objetiva y los resultados no deben generalizarse formalmente a la población (ej.: muestreo por conveniencia, por cuotas, a criterio o juicio, bola de nieve).

### Error de muestreo vs. errores no muestrales

| | Error de muestreo | Errores no muestrales |
|---|---|---|
| **Definición** | Diferencia entre el resultado obtenido en la muestra y el verdadero valor poblacional, debida únicamente al hecho de que se estudió solo una parte de la población (y no toda). | Errores que se producen durante el proceso de recolección, procesamiento o análisis de los datos, y que **no** están relacionados con el hecho de muestrear. |
| **Causa** | Variabilidad natural entre muestras (azar). | Fallas humanas o de procedimiento: mala redacción de preguntas, errores del entrevistador, no respuesta, errores de digitación, mentiras del informante, etc. |
| **Se presenta en** | Solo en estudios por muestreo. | Tanto en censos como en muestreos. |
| **Se puede medir/controlar** | Sí, mediante fórmulas estadísticas (se reduce aumentando el tamaño de muestra). | Es más difícil de medir y de controlar; requiere buen diseño del instrumento, capacitación de encuestadores y control de calidad. |


