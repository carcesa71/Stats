# Guía de Estudio: Medidas de Posición y Variabilidad

## 1. Propósito y uso de las medidas de posición

Las **medidas de posición** son valores que buscan resumir, con un solo número, dónde se ubica o "posiciona" el conjunto de datos, o partes de él, dentro de la escala de medición. Su propósito es:

- Sintetizar grandes volúmenes de datos en un valor representativo, facilitando su interpretación.
- Permitir la **comparación** entre distintos grupos, períodos o poblaciones.
- Servir de base para el cálculo de otras medidas (como las de variabilidad).
- Ubicar la posición relativa de una observación dentro del conjunto de datos.

Se dividen en dos grandes tipos:
- **Medidas de tendencia central**: buscan el "centro" de los datos (media, mediana, moda).
- **Medidas de posición no central (cuantiles)**: dividen el conjunto de datos ordenados en partes iguales (cuartiles, deciles, percentiles).

---

## 2. Interpretación de la Moda, la Mediana y los Cuantiles

### Moda (Mo)
Es el valor (o categoría) que **ocurre con mayor frecuencia** en el conjunto de datos.
- Puede calcularse con cualquier escala de medición, incluso la nominal.
- Un conjunto de datos puede ser **unimodal**, **bimodal** o **multimodal**, o incluso no tener moda si todos los valores tienen la misma frecuencia.
- **Interpretación**: representa el valor "típico" o más común; es útil cuando interesa saber cuál es la categoría o valor predominante (ej.: "la talla de zapato más vendida es la 38").

### Mediana (Md)
Es el valor que ocupa la **posición central** cuando los datos están ordenados de menor a mayor; divide al conjunto en dos mitades iguales (50% de los datos por debajo, 50% por encima).
- Requiere al menos escala ordinal.
- **Interpretación**: el 50% de las unidades tiene un valor igual o inferior a la mediana, y el otro 50% tiene un valor igual o superior (ej.: "la mediana salarial es ₡500.000" significa que la mitad de los trabajadores gana ₡500.000 o menos, y la otra mitad gana ₡500.000 o más).

### Cuantiles
Son valores que dividen un conjunto de datos ordenados en partes iguales. Los más usados son:
- **Cuartiles (Q1, Q2, Q3)**: dividen los datos en 4 partes iguales (cada una con el 25% de las observaciones). Q2 coincide con la mediana.
- **Deciles (D1...D9)**: dividen los datos en 10 partes iguales (cada una con el 10% de las observaciones).
- **Percentiles (P1...P99)**: dividen los datos en 100 partes iguales (cada una con el 1% de las observaciones).

**Interpretación general**: un percentil Pk indica que aproximadamente el k% de las observaciones tiene un valor igual o menor a ese punto (ej.: "un niño está en el percentil 90 de peso" significa que su peso es igual o mayor que el del 90% de los niños de su edad).

---

## 3. Cálculo e interpretación de la media aritmética simple y ponderada

### Media aritmética simple
Se calcula sumando todos los valores observados y dividiendo entre el número total de observaciones:

$$\bar{x} = \frac{\sum_{i=1}^{n} x_i}{n}$$

**Interpretación**: representa el valor "promedio" o el punto de equilibrio de los datos; es el valor que cada unidad tendría si el total se repartiera equitativamente entre todas.

### Media aritmética ponderada
Se utiliza cuando **no todos los valores tienen la misma importancia o peso** dentro del conjunto (por ejemplo, distintas cantidades de observaciones en cada categoría, o distintos pesos asignados a cada valor, como en el cálculo de notas):

$$\bar{x}_w = \frac{\sum_{i=1}^{n} w_i \, x_i}{\sum_{i=1}^{n} w_i}$$

donde $w_i$ es el peso (ponderación) asignado a cada valor $x_i$.

**Ejemplo**: el promedio de un curso donde el examen vale 60%, los trabajos 30% y la asistencia 10% se calcula como una media ponderada, no como una media simple de las tres notas.

**Interpretación**: representa un promedio que da más peso a los valores más relevantes o frecuentes, evitando distorsiones que ocurrirían si se tratara a todos los valores por igual.

---

## 4. Efectos de los valores extremos en las medidas de posición

- **Media aritmética**: es **muy sensible** a los valores extremos (atípicos o "outliers"), ya que estos afectan directamente la suma total. Un solo valor muy alto o muy bajo puede desplazar considerablemente la media, haciendo que deje de representar bien al "dato típico".
- **Mediana**: es **robusta** (poco sensible) ante valores extremos, porque depende solo de la posición central de los datos ordenados, no de su magnitud exacta.
- **Moda**: tampoco se ve afectada por valores extremos, ya que depende únicamente de la frecuencia.

**Regla práctica**: cuando el conjunto de datos tiene valores extremos o está muy asimétrico (sesgado), se recomienda utilizar la **mediana** en lugar de la media como medida representativa, ya que la media podría dar una impresión distorsionada del conjunto de datos.

---

## 5. El problema de la variabilidad y su importancia

Dos conjuntos de datos pueden tener la **misma media** (o mediana) y sin embargo ser muy diferentes entre sí en cuanto a qué tan dispersos o concentrados están sus valores alrededor de ese centro. A esto se le llama **variabilidad** o **dispersión**.

**Importancia**:
- Las medidas de posición por sí solas pueden ser engañosas si no se acompañan de una medida de variabilidad, ya que no dicen nada sobre qué tan homogéneos o heterogéneos son los datos.
- Permite evaluar la **confiabilidad** o **representatividad** de una medida de tendencia central: a menor variabilidad, más representativo es el promedio del conjunto de datos.
- Es clave en el control de calidad, la toma de decisiones bajo incertidumbre y la comparación de la consistencia entre grupos.

---

## 6. Medición de la variabilidad

### Recorrido o amplitud (Rango)
Es la medida de variabilidad más simple: la diferencia entre el valor máximo y el valor mínimo del conjunto de datos.

$$R = x_{max} - x_{min}$$

- Es fácil de calcular, pero **muy sensible a valores extremos** y no considera cómo se distribuyen los datos intermedios.

### Varianza
Mide el promedio de las desviaciones al cuadrado de cada dato respecto a la media. Al elevar al cuadrado, evita que las desviaciones positivas y negativas se cancelen entre sí.

- Población: $$\sigma^2 = \frac{\sum_{i=1}^{N}(x_i - \mu)^2}{N}$$
- Muestra: $$s^2 = \frac{\sum_{i=1}^{n}(x_i - \bar{x})^2}{n-1}$$

**Interpretación**: cuanto mayor es la varianza, mayor es la dispersión de los datos respecto a la media. Su principal desventaja es que queda expresada en **unidades al cuadrado**, lo que dificulta su interpretación directa (ej.: si los datos son en colones, la varianza queda en "colones al cuadrado").

### Desviación estándar (desviación típica)
Es la raíz cuadrada de la varianza:

$$s = \sqrt{s^2}$$

**Interpretación**: representa, en las **mismas unidades que los datos originales**, qué tanto se alejan en promedio los valores respecto a la media. Una desviación estándar pequeña indica datos muy concentrados cerca de la media; una desviación grande indica datos muy dispersos.

---

## 7. Interpretación del diagrama de caja (boxplot)

El **diagrama de caja** (box-and-whisker plot) es una representación gráfica que resume la distribución de los datos a partir de cinco valores clave (el "resumen de cinco números"):

1. Valor mínimo (o límite inferior, considerando atípicos).
2. Primer cuartil (Q1).
3. Mediana (Q2).
4. Tercer cuartil (Q3).
5. Valor máximo (o límite superior, considerando atípicos).

**Componentes y su interpretación**:
- **La caja**: va de Q1 a Q3 y representa el **rango intercuartílico (RIC = Q3 − Q1)**, es decir, contiene al 50% central de los datos.
- **La línea dentro de la caja**: marca la mediana; su posición dentro de la caja indica si hay simetría (centrada) o asimetría (desplazada hacia un lado) en la distribución.
- **Los "bigotes" (whiskers)**: se extienden desde la caja hasta los valores mínimo y máximo que no se consideran atípicos (normalmente hasta 1.5 veces el RIC desde cada cuartil).
- **Puntos fuera de los bigotes**: se consideran **valores atípicos (outliers)**.
- El **tamaño de la caja y de los bigotes** permite comparar visualmente la variabilidad y la simetría entre distintos grupos de datos.

---

## 8. Cálculo e interpretación del coeficiente de variación

El **coeficiente de variación (CV)** es una medida de variabilidad **relativa**, ya que expresa la desviación estándar como un porcentaje de la media:

$$CV = \frac{s}{\bar{x}} \times 100\%$$

**¿Por qué es útil?**
- La desviación estándar es una medida **absoluta**, expresada en las unidades originales de los datos, por lo que no permite comparar directamente la variabilidad entre conjuntos de datos con unidades distintas (ej.: peso vs. altura) o con medias muy diferentes (ej.: el salario de una empresa pequeña vs. una grande).
- El CV, al ser un valor **adimensional** (porcentaje), permite comparar la variabilidad relativa entre distintos conjuntos de datos, aunque tengan escalas o unidades diferentes.

**Interpretación**: 
- Un CV bajo indica que los datos son relativamente homogéneos (poca dispersión respecto a su media).
- Un CV alto indica mayor heterogeneidad relativa.
- Como referencia general (no una regla absoluta), suele considerarse que un CV menor al 15%-20% indica baja variabilidad, mientras valores más altos sugieren datos muy dispersos en relación con su media.

*Nota: el CV solo tiene sentido cuando la variable se mide en una escala de razón (con cero absoluto) y la media es distinta de cero, ya que de lo contrario el resultado puede ser engañoso o indefinido.*

---

*Guía elaborada como material de repaso. Si quieres, podemos continuar con ejemplos numéricos resueltos paso a paso (cálculo de media ponderada, varianza, o construcción de un diagrama de caja) para reforzar estos temas.*
