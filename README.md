# challenge-ds-tiendas-alura
# Análisis de Ventas de Tiendas

## Problemática

El desafío consiste en ayudar al señor Juan a decidir cuál de sus cuatro tiendas debe vender para invertir en un nuevo negocio. Para tomar esta decisión, se requiere un análisis de ventas y rendimiento de cada tienda.

Aspectos a evaluar son:

**Facturación total:** Determinar cuál tienda vende más.

**Categorías más populares:** Identificar qué productos se venden más en cada tienda.

**Promedio de evaluación de clientes:** Evaluar la satisfacción de los clientes en cada tienda.

**Productos más y menos vendidos:** Analizar cuáles son los productos que tienen mejor y peor desempeño en ventas.

**Costo promedio de envío:** Calcular el costo de envío desde cada tienda hasta los clientes.

Con esta información, el señor Juan podrá tomar una decisión informada sobre qué tienda es más eficiente y cuál es la menos eficiente, para en base a esto proceder con el cierre de la menos eficiente.

## Contenido

El análisis se divide en varias secciones, cada una abordando diferentes aspectos de las ventas:

1. **Análisis y Facturación**  
2. **Ventas por Categoría**  
3. **Calificación Promedio de Cada Tienda**  
4. **Productos Más y Menos Vendidos**  
5. **Envío Promedio por Tienda**  
6. **Dispersión Geográfica**  
7. **Precios Promedio por Tienda**  
8. **Ganancias por Categoría**  
9. **Ratios de Envío vs Precio de Tienda**  
10. **Conclusiones Finales**

## Metodología

Para cada sección del análisis, se han seguido los siguientes pasos generales:

1. **Hipótesis Inicial**: Se plantea una hipótesis sobre el comportamiento esperado de los datos.  
2. **Metodología**: Se describe el proceso utilizado para analizar los datos, incluyendo las funciones y técnicas aplicadas.  
3. **Resultados**: Se presentan los datos obtenidos de manera clara y concisa.  
4. **Conclusiones**: Se extraen conclusiones basadas en los resultados obtenidos.

## Resultados Clave

### 1. Análisis y Facturación

En este estudio se buscó poder obtener inicialmente las ganancias totales de cada tienda para posteriormente analizar los datos obtenidos.


**Hipótesis Inicial:**

Inicialmente se pensó que los productos de un mismo tipo, por ejemplo, una "cama box" podría tener el mismo valor cada vez que hubiese sido vendida, pero luego de hacer un análisis se llegó a la conclusión de que los artículos tenían precios distintos, ya fueran del mismo tipo o incluso perteneciendo a la misma categoría.

**Metodología:**

Debido a lo señalado anteriormente, se decidió sumar directamente la columna de ventas para poder obtener las ventas totales de cada tienda.

Los valores obtenidos fueron:


*   Tienda 1: $1150880400.0

*   Tienda 2: $1116343500.0

*   Tienda 3: $1098019600.0

*   Tienda 4: $1038375700.0



Gráficamente podemos verlo de la siguiente forma:

**Conclusión Estudio 1**

Claramente podemos ver que, si nos basamos solo en las ventas totales, sin tomar en cuenta ningún otro parámetro, la "Tienda 1" se destaca claramente sobre el resto, obteniendo una diferencia de "$112.504.700" en comparación al de peor rendimiento, la cual fue en este caso la "Tienda 4"


### 2. Ventas por Categoría

En este estudio se buscó analizar cuáles fueron las categorías que más ventas tuvieron, para poder ver cuáles eran los pilares en cuanto a ventas para cada tienda.


**Hipótesis Inicial:**

Inicialmente se pensó que cada tienda, dependiendo de varios factores como ubicación geográfica, vendedores, precios, entre muchos otros, iba a influir en la cantidad de ventas por categorías de cada tienda, presentando diferentes categorías destacadas en cada una.

**Metodología:**

Debido a lo señalado anteriormente, se decidió primero hacer un filtro en la columna "Categoría del Producto" para poder realizar una limpieza y evitar categorías repetidas, y así luego poder contar cada producto vendido asociado a una categoría en específico.

Los datos obtenidos fueron:

Categoría del Producto Tienda 1

*   Muebles: 465
*   Electrónicos: 448
*   Juguetes: 324
*   Electrodomésticos: 312
*   Deportes y diversión: 284
*   Instrumentos musicales: 182
*   Libros: 173
*   Artículos para el hogar: 171


Categoría del Producto Tienda 2

*   Muebles: 442
*   Electrónicos: 422
*   Juguetes: 313
*   Electrodomésticos: 305
*   Deportes y diversión: 275
*   Instrumentos musicales: 224
*   Libros: 197
*   Artículos para el hogar: 181

Categoría del Producto Tienda 3

*   Muebles: 499
*   Electrónicos: 451
*   Juguetes: 315
*   Electrodomésticos: 278
*   Deportes y diversión: 277
*   Libros: 185
*   Instrumentos musicales: 177
*   Artículos para el hogar: 177

Categoría del Producto Tienda 4

*   Muebles: 480
*   Electrónicos: 451
*   Juguetes: 338
*   Deportes y diversión: 277
*   Electrodomésticos: 254
*   Artículos para el hogar: 201
*   Libros: 187
*   Instrumentos musicales: 170

Gráficamente podemos verlo de la siguiente forma:

****Conclusión Estudio 2****

Como se puede observar, dentro de las categorías con más ventas destacan las Tiendas 1, 3 y 4. Si bien la Tienda 2 no destaca en ninguna de las categorías iniciales, tiene un alza importante en lo que son las 3 categorías con menos ventas, las cuales son "Instrumentos Musicales", "Libros" y "Artículos para el hogar".

Podemos notar que, si bien las 4 tiendas tienen un comportamiento similar en cuanto a las 3 categorías con más ventas, también podemos señalar lo siguiente:

1.   La Tienda 1 es la que generalmente tiene un comportamiento en cuanto a ventas más homogéneo, estando siempre dentro de las 2 o 3 primeras con más ventas por cada categoría.
2.   Si bien las Tiendas 3 y 4 tienen buenos comportamientos en cuanto a ventas por categoría en las 3 categorías principales, luego sufren una fuerte baja, lo cual podría explicar por qué son las 2 con menos ventas respecto al resto.
3.    Si bien la Tienda 4 sufre un alza importante en la cantidad de ventas en la categoría menos vendida ("Artículos para el hogar"), pareciera que esta categoría tiene ingresos muy bajos, lo cual hace que en el total de ventas esta alza no se vea reflejada.

### 3. Calificación Promedio de Cada Tienda

En este estudio se buscó obtener el promedio de la columna "Calificación", redondeando a 4 decimales, para luego poder hacer una comparación entre cada una de las tiendas.

**Hipótesis Inicial:**

Inicialmente se pensó que las tiendas con más ventas deberían ser las que presentarían mejores promedios de notas, dado que se podía inferir que las ventas reflejarían la conformidad de las personas con dichas tiendas.

**Metodología:**

Debido a lo señalado anteriormente, se decidió directamente utilizar las funciones mean() y round() para poder obtener los promedios de "Calificaciones" de cada tienda y ajustar la cantidad de decimales a la deseada, en este caso a 4.

Los datos obtenidos fueron:

*   Promedio Tienda 1: 3.9767
*   Promedio Tienda 2: 4.0373
*   Promedio Tienda 3: 4.0483
*   Promedio Tienda 4: 3.9958

Gráficamente podemos verlo de la siguiente forma:

**Conclusión Estudio 3**

Como se puede observar, la tienda "mejor calificada" es la Tienda 3, mientras que la peor es la Tienda 1. Al contrario de lo que pensábamos inicialmente, la cantidad de ventas y volumen de ventas no se ven reflejados en la satisfacción de los clientes, lo cual nos podría hacer pensar que las ventas de la Tienda 1 no dependen de los productos en sí, sino de factores externos como pueden ser vendedores, ubicación geográfica, etc.

### 4. Productos Más y Menos Vendidos

En este estudio se buscó tener más claridad sobre los productos más y menos vendidos de cada tienda, basado en los datos obtenidos desde las bases de datos entregadas.

**Hipótesis Inicial:**

Inicialmente se espera que los productos más vendidos tengan relación con las categorías más vendidas analizadas en el estudio 2, al igual que los productos menos vendidos deberían ir asociados a las categorías con menos ventas.

**Metodología:**

Se buscó traer todos los productos con sus respectivas cantidades, luego se generaron duplas para poder realizar un filtro que me indicara el producto más vendido y, a su vez, el menos vendido por cada tienda.

Los datos obtenidos fueron:


Productos Más Vendidos por Tienda:

|Tienda|Producto|Cantidades|
|------|--------|----------|
|Tienda 1|Microondas| 60 u. |
|Tienda 2|Iniciando en programación|65 u.|
|Tienda 3|Kit de bancas|57 u.|
|Tienda 4|Cama box|62 u.|

Productos Menos Vendidos por Tienda:

|Tienda|Producto|Cantidades|
|------|--------|----------|
|Tienda 1|Auriculares con micrófono| 33 u. |
|Tienda 2|Juego de mesa|32 u.|
|Tienda 3|Bloques de construcción|35 u.|
|Tienda 4|Guitarra eléctrica|33 u.|


Gráficamente podemos verlo de la siguiente forma:

**Conclusión Estudio 4**

Como se puede apreciar, los datos obtenidos de los artículos más y menos vendidos por cada tienda son congruentes respecto al análisis 2, en cuanto, generalmente, los productos más vendidos o menos vendidos corresponden a las categorías más o menos vendidas de cada tienda.

### 5. Envío Promedio por Tienda

En este estudio se buscó obtener el promedio de la columna "Costo de envío", para poder tener una idea de los costos de envío promedio de cada tienda.

**Hipótesis Inicial:**

La hipótesis inicial es que las tiendas tendrán promedios de envíos más altos dependiendo de la cantidad de ventas que tengan.

**Metodología:**

Debido a lo señalado anteriormente, se decidió directamente utilizar las funciones mean() y round() para poder obtener los promedios de "Costo de envío" de cada tienda y ajustar la cantidad de decimales a la deseada, en este caso a 4.

Los datos obtenidos fueron:

*   Envío Promedio Tienda 1: $26018.6096

*   Envío Promedio Tienda 2: $25216.2357

*   Envío Promedio Tienda 3: $24805.6804

*   Envío Promedio Tienda 4: $23459.4572

Gráficamente podemos verlo de la siguiente forma:

**Conclusión Estudio 5**

Tal como se esperaba, los promedios de los costos de envío se condicen con las ventas totales de cada tienda, por lo cual vemos que la Tienda 1 fue la que más vendió, seguida por la Tienda 2, Tienda 3 y finalmente la Tienda 4 respectivamente.

*Nota: Es importante tener en cuenta para este análisis que, si bien obtenemos un promedio de costo de envío, en ningún caso se aclara si el costo es asumido por el cliente o la tienda, con el fin de saber cuál es la ganancia total de la empresa en estos casos.*


### 6. Dispersión Geográfica

Se realiza este estudio para poder comprender la dispersión de las ventas de cada tienda, ya que es importante conocer cuánta área abarcan los vendedores de cada tienda y cómo puede esto influir positiva o negativamente en las ganancias de cada tienda.

**Hipótesis Inicial:**

Se piensa que las tiendas que tienen más ventas y mayores envíos promedio sean las que abarquen zonas más distantes de despachos.

**Metodología:**

Básicamente se toma una tienda completa, se agrupan por vendedores y se calcula la desviación estándar de la latitud y longitud de cada uno para cada tienda. Luego sumamos las desviaciones y calculamos la dispersión geográfica promedio para cada uno.

Los datos obtenidos fueron:



Tienda 1

| Vendedor | lat | lon | Dispersion Total|
|----------|-----|-----|-----------------|
|Beatriz Morales|1.832827|1.006599|2.83942|
|Blanca Ramirez|2.146864|1.041912|3.188776|
|Camila Rivera|2.539425|1.282224|3.821649|
|Felipe Santos|2.258005|1.183870|3.441875|
|Izabela de León|2.470557|1.394760|3.865317|
|Juan Fernandez|1.928816|1.186599|3.115415|
|Juliana Costa|2.284576|1.309608|3.594184|
|Lucas Olivera|1.966384|1.031781|2.998165|
|Maria Alfonso|1.815105|1.061503|2.876608|
|Mariana Herrera|2.762066|1.400138|4.162204|
|Pedro Gomez|2.626527|1.307780|3.934307|
|Rafael Acosta|2.688888|1.398675|4.087563|
|Santiago Silva|2.659459|1.250261|3.909721|
|Ángel Rodriguez|1.752578|1.027641|2.780218|



Tienda 2

| Vendedor | lat | lon | Dispersion Total|
|----------|-----|-----|-----------------|
|Beatriz Morales|2.172651|1.103784|3.276435|
|Blanca Ramirez|2.751452|1.299459|4.050911|
|Camila Rivera|2.319284|1.166676|3.485960|
|Felipe Santos|2.121760|1.095946|3.217706|
|Izabela de León|2.473285|1.258281|3.731566|
|Juan Fernandez|2.225615|1.124233|3.349848|
|Juliana Costa|2.500229|1.284961|3.785190|
|Lucas Olivera|2.286430|1.129089|3.415519|
|Maria Alfonso|2.622893|1.311259|3.934152|
|Mariana Herrera|2.155073|1.057206|3.212279|
|Pedro Gomez|2.355156|1.139119|3.494275|
|Rafael Acosta|2.382628|1.320609|3.703237|
|Santiago Silva|2.387906|1.128633|3.516539|
|Ángel Rodriguez|2.051042|1.097006|3.148048|

Tienda 3

| Vendedor | lat | lon | Dispersion Total|
|----------|-----|-----|-----------------|
|Beatriz Morales | 2.653183|  1.244759   |       3.897942|
|Blanca Ramirez | 2.150947|  1.139319  |        3.290266|
|Camila Rivera | 2.176740 | 1.070727   |       3.247466|
|Felipe Santos | 2.221588 | 1.160128 |         3.381716|
|Izabela de León | 2.375826 | 1.259846  |        3.635671|
|Juan Fernandez|  2.589467 | 1.235921  |        3.825389|
|Juliana Costa | 2.630421 | 1.385766  |        4.016186|
|Lucas Olivera|  2.486649 | 1.184418   |       3.671067|
|Maria Alfonso | 2.558297 | 1.253287 |        3.811583|
|Mariana Herrera | 2.349878 | 1.237898  |        3.587776|
|Pedro Gomez | 2.419873  |1.167361    |      3.587234|
|Rafael Acosta  |2.117155 |1.203376  |        3.320531|
|Santiago Silva|  2.758229 | 1.439802 |         4.198031|
|Ángel Rodriguez | 2.060488 | 1.106385 |         3.166873|


Tienda 4

| Vendedor | lat | lon | Dispersion Total|
|----------|-----|-----|-----------------|
|Beatriz Morales | 2.502157 | 1.214919     |     3.717076|
|Blanca Ramirez | 2.651609 | 1.201042    |      3.852651|
|Camila Rivera | 1.825061 | 1.028574     |     2.853635|
|Felipe Santos | 2.469973 | 1.426517     |     3.896490|
|Izabela de León | 2.112492 | 1.004878   |       3.117370|
|Juan Fernandez | 2.706133 | 1.272027    |      3.978159|
|Juliana Costa|  2.471409 | 1.184572     |     3.655980|
|Lucas Olivera | 2.525966 | 1.338404     |     3.864371|
|Maria Alfonso | 2.340784 | 1.221127    |      3.561911|
| Mariana Herrera | 2.562148  |1.306772  |        3.868920|
|Pedro Gomez | 2.404256 | 1.150513      |    3.554769|
|Rafael Acosta | 2.262630 | 1.044255     |     3.306885|
|Santiago Silva | 1.909183 | 1.171616   |       3.080799|
|Ángel Rodriguez | 2.203191 | 1.072129    |      3.275319|

Gráficamente podemos verlo de la siguiente forma:

**Conclusión Estudio 6**

Basándonos en algunos cálculos hechos en este estudio, los cuales se encuentran en la sección "**Eficiencia Relativa (Ventas por Unidad de Dispersión)**", podemos concluir lo siguiente:

1.   La Tienda 1 es la más eficiente, ya que vendió $331665821.33 por unidad de dispersión.

2.   La Tienda 3 es la menos eficiente, ya que apenas vendió $303320331.49 por unidad de dispersión.

Lo anterior nos demuestra que la eficiencia de la Tienda 3 no está siendo adecuada, ya que, a pesar de tener más ventas que la Tienda 4, al relacionarlo con su dispersión geográfica podemos notar que se queda atrás respecto a esta última.


### 7. Precios Promedio por Tienda

En este estudio se buscó conocer si el promedio de los precios de los productos por cada tienda podía influir o no significativamente en las ventas totales finales por cada tienda.

**Hipótesis Inicial:**

La hipótesis inicial es que las ventas promedio deberían ser similares entre las cuatro tiendas.

**Metodología:**

Lo que se hizo fue, por medio de la función "mean()", calcular el promedio de las columnas "Precio" de cada tienda, redondear a 4 decimales y luego comparar los valores obtenidos.

Los datos obtenidos fueron:

*   Precio Promedio Tienda 1: 487867.9101
*   Precio Promedio Tienda 2: 473227.4269
*   Precio Promedio Tienda 3: 465459.7711
*   Precio Promedio Tienda 4: 440362.8923

**Conclusión Estudio 7**

Basándonos en este estudio, podemos ver una variación de casi un 10% de los precios entre la Tienda 1 y la Tienda 4, lo cual podría implicar que los valores de los productos son más altos en la Tienda 1, afectando las ganancias totales finales, o que la cantidad de ventas de la Tienda 4 han sido productos de bajo costo, lo cual ha hecho que el promedio se vea distorsionado respecto al resto.

### 8. Ganancias por Categoría

En este estudio se buscó comprobar si existía una homogeneidad entre las categorías con más ventas entre las 4 tiendas y así descartar que fueran ciertos productos los que pudieran estar distorsionando los demás estudios.

**Hipótesis Inicial:**

La hipótesis inicial es que cada tienda tiene las mismas categorías con más ventas que las demás.

**Metodología:**

Lo que se hizo fue hacer una sumatoria de los precios de cada tienda, ordenarlas por categoría y luego mostrar ordenadas las categorías con más y menos ventas de cada tienda.

Los datos obtenidos fueron:

Tienda 1:

|Categorías| Ventas|
|-----------|--------|
|Electrónicos           |    429493500.0|
|Electrodomésticos       |   363685200.0|
|Muebles                  |  187633700.0|
|Instrumentos musicales    |  91299000.0|
|Deportes y diversión      |  39290000.0|
|Juguetes                   | 17995700.0|
|Artículos para el hogar |    12698400.0|
|Libros                   |    8784900.0|


Tienda 2:

|Categorías| Ventas|
|-----------|--------|
|Electrónicos        |       410831100.0|
|Electrodomésticos   |       348567800.0|
|Muebles             |       176426300.0|
|Instrumentos musicales|     104990300.0|
|Deportes y diversión  |      34744500.0|
|Juguetes              |      15945400.0|
|Artículos para el hogar|     14746900.0|
|Libros                  |    10091200.0|


Tienda 3:

|Categorías| Ventas|
|-----------|--------|
|Electrónicos           |    410775800.0|
|Electrodomésticos       |   329237900.0|
|Muebles                 |   201072100.0|
|Instrumentos musicales  |    77380900.0|
|Deportes y diversión    |    35593100.0|
|Juguetes                |    19401100.0|
|Artículos para el hogar |    15060000.0|
|Libros                  |     9498700.0|


Tienda 4:

|Categorías| Ventas|
|-----------|--------|
|Electrónicos            |   409476100.0|
|Electrodomésticos       |   283260200.0|
|Muebles                 |   192528900.0|
|Instrumentos musicales  |    75102400.0|
|Deportes y diversión    |    33350100.0|
|Juguetes                |    20262200.0|
|Artículos para el hogar |    15074500.0|
|Libros                  |     9321300.0|

**Conclusión Estudio 8**

Como se aprecia en los resultados, las categorías con más ventas no influyen directamente en las ventas totales, ya que dejando fuera la Tienda 1, las Tiendas 2, 3 y 4 tienen categorías con ventas similares si nos remitimos a las 3 primeras categorías con más ventas.

### 9. Ratios de Envío vs Precio de Tienda

En este estudio se buscó poder obtener el porcentaje del costo de envío en relación con el precio de cada producto de cada tienda.

**Hipótesis Inicial:**

Basándonos solo en el estudio de las ventas totales de cada tienda, podríamos esperar que esta relación costo_envío/precio por cada producto pudiera entregarnos una relación más favorable en la Tienda 1 y menos favorable en la Tienda 4.

**Metodología:**

Lo que se hizo fue calcular qué porcentaje del valor del producto era el costo de envío que tenía asociado y almacenarlo en una nueva columna, la cual luego sería promediada para poder comparar el resultado entre las 4 tiendas.

Los datos obtenidos fueron:

*   Tienda 1: 5.52%
*   Tienda 2: 5.61%
*   Tienda 3: 5.37%
*   Tienda 4: 5.54%

**Conclusión Estudio 9**

Como se aprecia en los resultados, la tienda 2 y la tienda 4 son las que tienen peor relación entre costo de envío y precio de producto. El problema que se presenta para la tienda 4 es que además tiene la peor venta total de las 4 tiendas, por lo cual que el precio de envío sea alto pone una alarma importante financieramente hablando.

## Conclusiones Finales

Basado en los estudios anteriores, si realizamos un análisis por tienda encontramos lo siguiente:

- **Tienda 1:** Debe mejorar la eficiencia entre sus ventas y sus precios de envío para obtener mayores ingresos. Por otro lado, debe implementar estrategias de marketing enfocadas en mejorar la atención a los clientes. Lo que la favorece es que, a pesar de todo lo anterior, es la tienda que más territorio abarca y la que más ingresos genera de las 4 tiendas.

- **Tienda 2:** Posee unos ingresos respetables al ser la 2da con mayores ingresos de las 4. Debe enfocarse en la relación entre costos de envío y precio de los productos, para que sus ingresos sean mayores, ya que es su debilidad más grande actualmente.

- **Tienda 3:** Es por lejos la tienda con mejores calificaciones de las 4 y además su relación entre costos de envío y precio de productos es la mejor de las 4 tiendas. Su principal debilidad es el poco territorio que abarca con sus tiendas, debiendo enfocarse en mejorar este problema, sin olvidar tener en cuenta revisar los precios de sus productos.

- **Tienda 4:** Si bien tiene los promedios de envíos más bajos y los precios más bajos, esto podría significar que o su enfoque está siendo equivocado en cuanto a los productos que está potenciando, o que literalmente sus estructuras de precios no son las adecuadas para poder ver reflejado esto en sus ganancias. De hecho, de las 4 tiendas, es la que posee menores ganancias. Además, a lo anterior debemos sumar que es la 2da tienda con peor calificación de las 4, por lo cual la preferencia de los clientes será baja. A esto debemos sumar que, a pesar de vender menos, la relación entre costos de envío y precio de los productos es la 2da peor, generando que las ganancias sean aún más bajas.

**Decisión Final:**

Se sugiere cerrar la tienda 4 por los siguientes motivos:

- **Bajos ingresos totales:** Ni siquiera alcanza a superar la barrera de los $1.100.000.000.

- **Bajos Precios:** Hacen que sea cuestionable el manejo de la empresa desde el punto de vista financiero, ya que se observan precios bajos y, a la vez, bajos ingresos totales, lo cual podría indicar un margen bajo también.

- **Relación Costo envío y Precio producto:** Su relación entre costo de envío y precio de producto es de las 2 peores, lo cual indica que el margen, de asumirlo la tienda, será menor y, en caso de asumirlo el cliente, indicará un factor en contra para la tienda, ya que no necesariamente estarán dispuestos a asumir un costo alto de envío.

- **Falta de ventajas competitivas:** A pesar de tener un producto con muchas ventas como lo son las "camas box", esta no pertenece a las categorías que mayores ganancias entregan a la tienda, ya que esta pertenece a la categoría "muebles" y la categoría con mayores ganancias es la de "Electrónicos"

## Requisitos

- Python 3.x  
- pandas  
- matplotlib (para visualización de datos)

## Instalación

Para instalar las dependencias necesarias, ejecute:

```bash
pip install pandas matplotlib
