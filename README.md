# Análisis de Datos de Pedidos de Instacart

Este proyecto consiste en un análisis exploratorio de datos utilizando un conjunto de datos de pedidos de Instacart, una plataforma de entregas de comestibles en línea. El objetivo es limpiar los datos y explorar los hábitos de compra de los clientes de Instacart a través de un análisis detallado.

## Datasets Utilizados

- **instacart_orders.csv**: Información sobre cada pedido realizado en la plataforma.
- **products.csv**: Detalles sobre los productos disponibles en Instacart.
- **order_products.csv**: Información sobre los productos incluidos en cada pedido.
- **aisles.csv**: Categorías de pasillos donde se encuentran los productos.
- **departments.csv**: Departamentos de víveres a los que pertenecen los productos.

## Pasos Realizados

### 1. Preprocesamiento de Datos
- **Verificación y Corrección de Tipos de Datos**: Aseguramos que todas las columnas tengan los tipos de datos correctos, como enteros para las columnas de ID.
- **Tratamiento de Valores Ausentes**: Identificación y manejo de valores ausentes, incluyendo la justificación de los métodos utilizados para completarlos o eliminarlos.
- **Eliminación de Duplicados**: Detección y eliminación de registros duplicados para asegurar la integridad de los datos.

### 2. Análisis Exploratorio

#### A. Verificación y Visualización Inicial
- **Verificación de Rango de Valores**: Aseguramos que las columnas `order_hour_of_day` y `order_dow` tengan valores razonables.
- **Gráfico de Pedidos por Hora del Día**: Visualización del número de pedidos realizados en cada hora del día.
- **Gráfico de Pedidos por Día de la Semana**: Análisis de los días en que los clientes realizan más pedidos.
- **Distribución del Tiempo entre Pedidos**: Visualización y comentario sobre el tiempo que los clientes esperan para hacer su próximo pedido.

#### B. Distribuciones y Productos Populares
- **Comparación entre Miércoles y Sábados**: Análisis de las diferencias en la hora del día en que se hacen pedidos en miércoles y sábados.
- **Distribución del Número de Pedidos por Cliente**: Visualización de cuántos pedidos realizan los clientes en total.
- **Productos Más Populares**: Identificación de los 20 productos más frecuentemente pedidos.

#### C. Análisis de Reordenes y Primeros Artículos en el Carrito
- **Distribución de Artículos por Pedido**: Análisis de cuántos artículos se incluyen típicamente en un pedido.
- **Productos Reordenados**: Identificación de los 20 productos más frecuentemente reordenados.
- **Proporción de Reordenes por Producto**: Cálculo de la proporción de veces que un producto es reordenado.
- **Proporción de Reordenes por Cliente**: Análisis de la frecuencia con que los clientes reordenan productos.
- **Primeros Artículos en el Carrito**: Identificación de los 20 productos que más veces se añaden primero al carrito de compras.

## Conclusión General

Este análisis proporciona una visión detallada de los patrones de compra de los clientes de Instacart, lo que puede ser útil para optimizar estrategias de marketing y mejorar la experiencia del usuario en la plataforma.

