# Análisis de Datos de Instacart

## Descripción del Proyecto

Este proyecto se centra en el análisis de datos de Instacart, una plataforma de entregas de comestibles. El objetivo es limpiar los datos proporcionados y preparar un informe detallado sobre los hábitos de compra de los clientes de Instacart.

Los datos incluyen cinco archivos CSV con información sobre pedidos, productos, pasillos y departamentos. A través de este análisis, se busca obtener información valiosa sobre el comportamiento de compra de los usuarios y cómo se distribuyen los productos y pedidos.

## Datos

El conjunto de datos se compone de los siguientes archivos:

- **`instacart_orders.csv`**: Información sobre cada pedido realizado en Instacart.
  - `order_id`: Identificador único del pedido.
  - `user_id`: Identificador único del cliente.
  - `order_number`: Número de veces que el cliente ha hecho un pedido.
  - `order_dow`: Día de la semana en que se realizó el pedido (0 si es domingo).
  - `order_hour_of_day`: Hora del día en que se realizó el pedido.
  - `days_since_prior_order`: Número de días desde el pedido anterior del cliente.

- **`products.csv`**: Información sobre cada producto disponible en Instacart.
  - `product_id`: Identificador único del producto.
  - `product_name`: Nombre del producto.
  - `aisle_id`: Identificador único del pasillo.
  - `department_id`: Identificador único del departamento.

- **`order_products.csv`**: Información sobre los productos incluidos en cada pedido.
  - `order_id`: Identificador único del pedido.
  - `product_id`: Identificador único del producto.
  - `add_to_cart_order`: Orden en que el artículo fue añadido al carrito.
  - `reordered`: 0 si el producto no se había pedido antes, 1 si se había pedido.

- **`aisles.csv`**: Información sobre las categorías de pasillos de víveres.
  - `aisle_id`: Identificador único del pasillo.
  - `aisle`: Nombre del pasillo.

- **`departments.csv`**: Información sobre los departamentos de víveres.
  - `department_id`: Identificador único del departamento.
  - `department`: Nombre del departamento.

## Instrucciones para Completar el Proyecto

### Paso 1: Exploración de Datos

- Abre los archivos de datos y examina el contenido general de cada tabla.
- Ten en cuenta los formatos no estándar de los archivos CSV. Establece los argumentos adecuados en `pd.read_csv()` para leer los datos correctamente.
- Para `order_products.csv`, usa `show_counts=True` al llamar a `info()` para imprimir los recuentos no nulos si el DataFrame es muy grande.

### Paso 2: Preprocesamiento de Datos

- Verifica y corrige los tipos de datos, asegurándote de que las columnas de ID sean numéricas.
- Identifica y completa los valores ausentes.
- Identifica y elimina los valores duplicados.
- Explica los problemas encontrados, cómo los abordaste y por qué elegiste esos métodos.

### Paso 3: Análisis Exploratorio de Datos

#### [A] Análisis Básico

1. Verifica la validez de las columnas `order_hour_of_day` y `order_dow`.
2. Crea un gráfico que muestre el número de pedidos por hora del día.
3. Crea un gráfico que muestre la cantidad de pedidos por día de la semana.
4. Crea un gráfico que muestre el tiempo que las personas esperan para hacer su próximo pedido. Comenta los valores mínimos y máximos.

#### [B] Análisis Comparativo

1. Compara las distribuciones de `order_hour_of_day` entre miércoles y sábados mediante histogramas.
2. Traza la distribución del número de pedidos por cliente.
3. Identifica los 20 productos más frecuentemente pedidos (incluye ID y nombre).

#### [C] Análisis Detallado

1. Determina el número promedio de artículos por pedido y su distribución.
2. Identifica los 20 artículos más frecuentemente reordenados (incluye nombres e ID).
3. Calcula la proporción de reordenes para cada producto (tabla con ID, nombre y proporción).
4. Calcula la proporción de productos reordenados por cada cliente.
5. Identifica los 20 artículos que más frecuentemente se añaden primero al carrito (incluye ID, nombre y número de veces).

