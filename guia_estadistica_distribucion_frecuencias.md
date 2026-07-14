# Guía de Estudio: Distribuciones de Frecuencias

## 1. Definición de distribución de frecuencias

Una **distribución de frecuencias** es un arreglo (generalmente en forma de tabla) que organiza un conjunto de datos, mostrando las distintas categorías o valores que toma una variable junto con el número de veces que cada uno se repite (su frecuencia).

- Su propósito es **resumir y organizar** los datos en bruto para facilitar su lectura, análisis e interpretación.
- Se puede construir para variables **cualitativas** (categorías) o **cuantitativas** (valores numéricos, ya sea datos sin agrupar o agrupados en intervalos de clase).
- Cuando la variable es cuantitativa continua o tiene muchos valores distintos, los datos suelen agruparse en **intervalos de clase**, cada uno con su respectivo **límite inferior**, **límite superior**, **marca de clase** (punto medio) y **amplitud**.

---

## 2. Frecuencias absolutas y relativas, simples y acumuladas

### Frecuencia absoluta simple ($f_i$)
Es el **número de veces** que se repite (o de observaciones que caen en) cada categoría o intervalo de clase.

- **Interpretación**: indica cuántas unidades estadísticas pertenecen a esa categoría/intervalo específico (ej.: "15 estudiantes obtuvieron una nota entre 80 y 90").
- La suma de todas las frecuencias absolutas simples debe ser igual al total de observaciones ($n$): $\sum f_i = n$.

### Frecuencia relativa simple ($h_i$)
Es la proporción (o porcentaje) que representa cada frecuencia absoluta respecto al total de observaciones:

$$h_i = \frac{f_i}{n}$$

- **Interpretación**: indica qué proporción (o %) del total de datos cae en esa categoría/intervalo (ej.: "el 25% de los estudiantes obtuvo una nota entre 80 y 90"). Es útil porque permite comparar distribuciones de distinto tamaño ($n$), algo que la frecuencia absoluta no permite directamente.
- La suma de todas las frecuencias relativas simples debe ser igual a 1 (o 100% si se expresa en porcentaje): $\sum h_i = 1$.

### Frecuencia absoluta acumulada ($F_i$)
Es la suma progresiva (acumulación) de las frecuencias absolutas simples, desde la primera categoría/intervalo hasta la categoría/intervalo en cuestión:

$$F_i = f_1 + f_2 + \dots + f_i$$

- **Interpretación**: indica cuántas observaciones tienen un valor **igual o menor** (o, según cómo se defina, hasta cierto punto) que el límite superior de esa categoría/intervalo (ej.: "40 estudiantes obtuvieron una nota de 90 o menos").
- La frecuencia absoluta acumulada de la última categoría/intervalo siempre es igual a $n$.

### Frecuencia relativa acumulada ($H_i$)
Es la suma progresiva de las frecuencias relativas simples, o equivalentemente, la frecuencia absoluta acumulada dividida entre $n$:

$$H_i = \frac{F_i}{n}$$

- **Interpretación**: indica qué **proporción (o %)** de las observaciones tiene un valor igual o menor que el límite superior de esa categoría/intervalo (ej.: "el 80% de los estudiantes obtuvo una nota de 90 o menos"). Es la base para calcular cuantiles (cuartiles, percentiles, etc.) a partir de datos agrupados.
- La frecuencia relativa acumulada de la última categoría/intervalo siempre es igual a 1 (o 100%).

### Tabla resumen

| Tipo de frecuencia | Fórmula / cálculo | ¿Qué responde? |
|---|---|---|
| Absoluta simple ($f_i$) | Conteo directo | ¿Cuántos casos hay en esta categoría? |
| Relativa simple ($h_i$) | $f_i / n$ | ¿Qué proporción representa esta categoría? |
| Absoluta acumulada ($F_i$) | Suma acumulada de $f_i$ | ¿Cuántos casos hay hasta este punto? |
| Relativa acumulada ($H_i$) | Suma acumulada de $h_i$ (o $F_i/n$) | ¿Qué proporción hay hasta este punto? |

---

## 3. Representación gráfica de las distribuciones de frecuencias

### Histograma
Es un gráfico de **barras contiguas** (sin espacio entre ellas), utilizado para representar la distribución de frecuencias de una **variable cuantitativa continua** agrupada en intervalos de clase.

- En el **eje horizontal (x)** se ubican los límites (o marcas de clase) de los intervalos.
- En el **eje vertical (y)** se ubica la frecuencia (absoluta o relativa) de cada intervalo.
- La **altura** de cada barra es proporcional a la frecuencia del intervalo que representa.
- Las barras van **unidas** (sin separación), a diferencia de un gráfico de barras para variables cualitativas, precisamente porque la variable es continua y los intervalos son consecutivos.

**Interpretación**: la forma del histograma permite identificar rápidamente:
- Dónde se concentra la mayor parte de los datos (los intervalos con barras más altas).
- Si la distribución es **simétrica** o **asimétrica** (sesgada a la izquierda o a la derecha).
- Si existen valores atípicos o intervalos con muy poca frecuencia.
- El número de "modas" o picos (unimodal, bimodal, etc.).

### Polígono de frecuencias
Es un **gráfico de líneas** que se construye uniendo con segmentos rectos los puntos correspondientes a la **marca de clase** (punto medio) de cada intervalo con su respectiva frecuencia (absoluta o relativa).

- Se suele "cerrar" el polígono añadiendo un intervalo ficticio de frecuencia cero antes del primero y después del último, para que la figura toque el eje horizontal en ambos extremos.
- Es equivalente al histograma en cuanto a la información que representa, pero es más útil para **comparar dos o más distribuciones** en un mismo gráfico (superponiendo varios polígonos), algo que resulta más difícil de hacer claramente con histogramas superpuestos.

**Interpretación**: igual que el histograma, permite visualizar la forma general de la distribución (simetría, sesgo, concentración de datos, modas), pero con la ventaja adicional de facilitar la comparación visual entre grupos.

### Polígono de frecuencias acumuladas (ojiva)
Es un gráfico de líneas que representa las **frecuencias acumuladas** (absolutas o relativas) en función de los **límites superiores** de cada intervalo de clase.

- Es una curva creciente (nunca decrece), ya que las frecuencias acumuladas nunca disminuyen.
- **Interpretación**: permite leer directamente, para cualquier valor del eje horizontal, cuántas observaciones (o qué proporción) se encuentran por debajo de ese valor. Es la herramienta gráfica utilizada para estimar cuantiles (mediana, cuartiles, percentiles) de forma visual.

---

---

## 4. Ejemplo resuelto: construcción de una tabla de frecuencias

**Datos**: se registraron las edades (en años) de 20 personas que visitaron una clínica:

```
19, 22, 25, 23, 30, 28, 21, 35, 24, 27,
33, 26, 29, 20, 31, 24, 28, 22, 26, 32
```

### Paso 1: Determinar el número de intervalos y su amplitud

Un criterio común (Regla de Sturges u otra aproximación práctica) sugiere entre 5 y 7 intervalos para este tamaño de muestra. Usaremos **5 intervalos**.

- Rango: $R = x_{max} - x_{min} = 35 - 19 = 16$
- Amplitud aproximada de cada intervalo: $c = R / \text{n° intervalos} = 16 / 5 = 3.2 \approx 4$

### Paso 2: Construir la tabla de distribución de frecuencias

| Intervalo (edad) | Marca de clase | $f_i$ | $h_i$ | $F_i$ | $H_i$ |
|---|---|---|---|---|---|
| 19 – 23 | 21 | 5 | 0.25 | 5 | 0.25 |
| 23 – 27 | 25 | 6 | 0.30 | 11 | 0.55 |
| 27 – 31 | 29 | 5 | 0.25 | 16 | 0.80 |
| 31 – 35 | 33 | 3 | 0.15 | 19 | 0.95 |
| 35 – 39 | 37 | 1 | 0.05 | 20 | 1.00 |
| **Total** | | **20** | **1.00** | | |

*(Convención usada: el límite inferior se incluye y el superior no, excepto en el último intervalo.)*

### Paso 3: Interpretar los resultados

- **Frecuencia absoluta simple**: 6 personas tienen edades entre 23 y 27 años (el intervalo más frecuente).
- **Frecuencia relativa simple**: el 30% de las personas encuestadas tiene edades entre 23 y 27 años.
- **Frecuencia absoluta acumulada**: 16 personas tienen menos de 31 años.
- **Frecuencia relativa acumulada**: el 80% de las personas tiene menos de 31 años (dato útil, por ejemplo, para estimar el tercer cuartil).

### Paso 4: Esbozo del histograma y el polígono

- **Histograma**: se dibujarían 5 barras contiguas (sin espacio entre ellas) sobre el eje horizontal (edad), con alturas de 5, 6, 5, 3 y 1 respectivamente. La barra más alta sería la del intervalo 23–27, mostrando que ahí se concentra la mayor parte de los datos.
- **Polígono de frecuencias**: se marcarían puntos en (21, 5), (25, 6), (29, 5), (33, 3) y (37, 1), uniéndolos con líneas rectas, y "cerrando" la figura con puntos de frecuencia 0 en las marcas de clase ficticias 17 y 41.
- **Forma de la distribución**: al ser mayor la frecuencia en los intervalos intermedios-bajos y disminuir hacia la derecha, la distribución muestra un **sesgo hacia la derecha (asimetría positiva)**: hay pocas personas de mayor edad que "alargan la cola" del gráfico hacia la derecha.

---

## 5. Ejemplo adicional breve: variable cualitativa

Si en lugar de edades se hubiera preguntado el **tipo de sangre** a las mismas 20 personas, y se obtuvieran los resultados: O (9 personas), A (6 personas), B (3 personas), AB (2 personas), la tabla de frecuencias sería:

| Tipo de sangre | $f_i$ | $h_i$ |
|---|---|---|
| O | 9 | 0.45 |
| A | 6 | 0.30 |
| B | 3 | 0.15 |
| AB | 2 | 0.10 |
| **Total** | **20** | **1.00** |

Aquí **no tiene sentido calcular frecuencias acumuladas** ($F_i$, $H_i$), porque el tipo de sangre es una variable **nominal** (sin orden lógico entre categorías) — acumular "hasta" un tipo de sangre no tiene interpretación válida. Tampoco se usaría un histograma, sino un **gráfico de barras** (con espacio entre ellas) o un gráfico circular (de pastel).

---

*Guía elaborada como material de repaso. Si quieres, podemos trabajar otro ejemplo con datos distintos, calcular la mediana o algún cuartil a partir de esta tabla agrupada, o pasar a los siguientes temas del curso.*
