# 💻  Ejercicio de data wrangling y visualización en una de plataforma de entregas 🏃

## 📋 Descripción
Análisis de patrones de compra en supermercados mediante data wrangling y visualización. Se procesaron múltiples datasets con problemas de calidad (duplicados, valores nulos, inconsistencias) para identificar tendencias de comportamiento de clientes: horarios pico de compra, días preferidos y frecuencia de pedidos

## 🎯 Objetivos
- Limpiar y procesar datos como valores nulos, duplicados, incosistencias 
- Identificar patrones de compra por horario y día de la semana
- Analizar la relación entre productos, pasillos y departamentos
- Detectar y corregir inconsistencias en los datos
- Ver hábitos de consumo
## 📊 Datasets Utilizados
- **instacart_orders.csv**: Información de pedidos (fecha, hora, usuario)
- **products.csv**: Catálogo de productos
- **order_products.csv**: Relación pedidos-productos
- **aisles.csv**: Información de pasillos
- **departments.csv**: Información de departamentos

## 🔧 Tecnologías
## 🔧 Tecnologías
Entorno de desarrollo:
- Jupyter Notebook
- Python 3.9.19
### Líbrerias:
- Pandas
- Matplotlib
- Numpy
- Matplotlib
- Scipy.stats - mannwhitneyu

## 📈 Conclusión
- Se decidio trabajar la variable de llamadas perdidas, ya que puede reflejar tambien el problema del alto porcentaje de tiempo de espera (el promedio de tiempo de espera es de 215 min y una desviacion estandar de 504, un minimo de 0 y un máximo de 5907, esto nos indica una diferencia enorme entre operadores y a su vez que hay valores totalmente extremos.), ya que clientes que no esperaron, se finaliza como llamada perdida. Tambien se hizo un filtrado de operadores, se filtraron las llamadas que no fueron asignadas a ningun operador, a los operadores que solo reciben y a los que solo hacen llamadas por la probabilidad de que tienen un rol específico como cobranza/ ventas / atencion al cliente. Se limito a analizar a 544 operadores que reciben y hacen llamadas, nombrados operadores mixtos. El promedio de llamadas perdidas entre estos operadores es del 32%.

- El planteamiento fue que, sí había diferencias significativa en las llamadas perdidas entre operadores mixtos que están por encima del 32% vs los operadores que estan por debajo del 32% y el resultado fue que si hay una diferencia estadísticamente significativa Estadístico U: 73728.0, Valor p: 2.7849075827387667e-90 (muy pequeño).

- Posteriormente se comparo la media vs la mediana para explicarlo con estadística descriptiva y se observo que los operadores mixtos que superan el umbral del 32% de llamadas perdidas tienen una mediana de 38.67%, mientras que los que están por debajo tienen una mediana de 23.24%. Esta diferencia de 15.43 puntos porcentuales es estadísticamente significativa.

- Los dos grupos de operadores tienen comportamientos claramente diferentes en cuanto a llamadas perdidas, confirmando que el umbral del 32% efectivamente separa operadores con diferentes niveles de desempeño.

