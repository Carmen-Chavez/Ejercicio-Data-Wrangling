# 🖥️ Análisis de Datos de Call Center

## 📋 Descripción
En una plataforma de entregas de comestibles donde la clientela puede registrar un pedido y hacer que se lo entreguen, similar a Uber Eats y Door Dash. El conjunto de datos con el que se trabajo, tiene modificaciones del original. Se redujo el tamaño del conjunto para que los cálculos se hicieran más rápido y se introdujeron valores ausentes y duplicados. Se tuvo cuidado de conservar las distribuciones de los datos originales cuando se hicieron los cambios.

## 🎯 Objetivos
- Manipulación de datos (data wrangling).
- Mejores días de venta.
- Horario pico en pedidos.
- Productos mas vendidos.
- Productos recomprados.

## 📊 Datasets Utilizados
- **instacart_orders.csv**:
- 'order_id': número de ID que identifica de manera única cada pedido.
- 'user_id': número de ID que identifica de manera única la cuenta de cada cliente.
- 'order_number': el número de veces que este cliente ha hecho un pedido.
- 'order_dow': día de la semana en que se hizo el pedido (0 si es domingo).
- 'order_hour_of_day': hora del día en que se hizo el pedido.
- 'days_since_prior_order': número de días transcurridos desde que este cliente hizo su pedido anterior.
- **products.csv**:
- 'order_id': número de ID que identifica de manera única cada pedido.
- 'product_id': número ID que identifica de manera única cada producto.
- 'add_to_cart_order': el orden secuencial en el que se añadió cada artículo en el carrito.
- 'reordered': 0 si el cliente nunca ha pedido este producto antes, 1 si lo ha pedido.
-**order_products.csv**:
- 'order_id': número de ID que identifica de manera única cada pedido.
- 'product_id': número ID que identifica de manera única cada producto.
- 'add_to_cart_order': el orden secuencial en el que se añadió cada artículo en el carrito.
- 'reordered': 0 si el cliente nunca ha pedido este producto antes, 1 si lo ha pedido.
-**aisles.csv**:
- 'aisle_id': número ID que identifica de manera única cada categoría de pasillo de víveres.
- 'aisle': nombre del pasillo.
**departments.csv**:
- 'department_id': número ID que identifica de manera única cada departamento de víveres.
- 'department': nombre del departamento.

## 🔧 Tecnologías
Entorno de desarrollo:
- Jupyter Notebook.
- Python 3.9.19.
### Líbrerias:
- Pandas.
- Matplotlib.
