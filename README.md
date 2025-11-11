#  Laboratorio Práctico: ETL y Análisis Exploratorio de Datos (EDA)

##  Descripción del Proyecto

Este proyecto corresponde al **Laboratorio 1 de la Especialización en Análisis de Datos**, cuyo objetivo es aplicar de forma integrada las competencias adquiridas durante el curso, desarrollando un proceso completo de análisis que incluye:

- **Extracción, Transformación y Carga (ETL)** de un conjunto de datos reales.
- **Análisis Exploratorio de Datos (EDA)** con Python y pandas.
- **Interpretación analítica** mediante la formulación de tres preguntas de negocio basadas en la exploración.
- **Publicación en GitHub** con ejecución directa en Google Colab.

---

##  Acceso al Notebook

Podés abrir y ejecutar el notebook directamente en Google Colab desde el siguiente enlace:

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1NRSmIvWs1jU6NZWSHxqzF5ni3eu2W50T?usp=sharing)

---

##  Dataset Utilizado

**Fuente:** Archivo local `productos.csv`  
**Descripción:** Dataset con información de productos comercializados, incluyendo marca, presentación, precios de lista y precios promocionales.  
**Columnas principales:**
- `productos_descripcion`: Nombre del producto.  
- `productos_marca`: Marca del producto.  
- `productos_precio_lista`: Precio base sin descuento.  
- `productos_precio_unitario_promo1`: Precio con promoción aplicada.  
- `productos_cantidad_presentacion`: Cantidad o volumen de presentación del producto.  

---

##  1. Proceso ETL

###  Extracción
Se importó el archivo CSV al entorno de trabajo en Google Colab utilizando `pandas.read_csv()`.

```python
df = pd.read_csv('/content/productos.csv', sep='|')


