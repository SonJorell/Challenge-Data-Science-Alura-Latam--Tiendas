# 📊 Desafío Alura Store: Análisis de Rendimiento y Toma de Decisiones

Este proyecto consiste en un análisis integral de datos utilizando **Python** y **Pandas** para evaluar el desempeño de cuatro tiendas de la cadena "Alura Store". El objetivo final es proporcionar una recomendación basada en datos para decidir qué unidad de negocio debe ser vendida para financiar un nuevo emprendimiento.



## 🎯 Propósito del Análisis
El Sr. Juan necesita identificar la tienda con menor rendimiento. Para ello, nos hemos enfocado en cinco pilares métricos fundamentales:
1. **Facturación Total:** ¿Qué tienda genera más ingresos brutos?
2. **Popularidad de Categorías:** ¿Cuáles son los productos que mueven el inventario?
3. **Satisfacción del Cliente:** Análisis de evaluaciones (estrellas) por tienda.
4. **Rotación de Productos:** Identificación de los productos más y menos vendidos.
5. **Eficiencia Logística:** Cálculo del costo promedio de envío por tienda.

## 🏗️ Estructura del Proyecto
El proyecto está organizado de la siguiente manera para garantizar la reproducibilidad:

* `AluraStoreLatam.ipynb`: Notebook de Google Colab con todo el código de procesamiento, limpieza y visualización.
* `tienda_1.csv` a `tienda_4.csv`: Bases de datos individuales por tienda que contienen registros de ventas, precios, costos y coordenadas geográficas.
* `README.md`: Documentación del proyecto (este archivo).



## 📈 Metodología e Insights Obtenidos

### 1. Análisis Financiero
Se calculó la facturación total mediante la suma de la columna `Precio`:
$$Ingreso = \sum_{i=1}^{n} (Precio_i)$$
* **Insight:** La **Tienda 1** lidera en ingresos, mientras que la **Tienda 4** muestra la facturación más baja del grupo, situándose por debajo de los mil millones de pesos.

### 2. Satisfacción y Logística
Cruzamos el promedio de calificación con el costo de envío.
* **Insight:** La **Tienda 3** posee la mejor reputación (4.04 ⭐). Curiosamente, la Tienda 4 tiene el costo de envío más bajo, pero esto no se traduce en un mayor volumen de ventas, sugiriendo una falta de tracción en su mercado local.

### 3. Visualizaciones
El proyecto incluye:
* **Gráficos de Barras:** Para comparar ingresos y costos de envío.
* **Gráficos de Líneas:** Para observar la tendencia de calificaciones.
* **Gráficos de Dispersión:** Para mapear la distribución geográfica de las ventas.



## 🚀 Instrucciones para Ejecutar el Notebook

Para replicar este análisis, sigue estos pasos:

1.  **Entorno:** Abre [Google Colab](https://colab.research.google.com/).
2.  **Carga de Datos:** Sube los archivos `.csv` (tienda_1 a tienda_4) a la sección de archivos de la sesión o utiliza los enlaces de GitHub proporcionados en el notebook.
3.  **Dependencias:** Asegúrate de tener instaladas las librerías necesarias (vienen por defecto en Colab):
    ```python
    import pandas as pd
    import matplotlib.pyplot as plt
    import seaborn as sns
    ```
4.  **Ejecución:** Ejecuta las celdas en orden secuencial. La última celda generará automáticamente el informe final y la recomendación estratégica.

---
**Recomendación Final:** Tras el análisis, se sugiere la venta de la **Tienda 4** debido a su menor rentabilidad comparativa y bajo volumen de ventas en categorías clave.
