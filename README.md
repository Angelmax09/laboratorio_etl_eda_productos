 Laboratorio Práctico — ETL & Análisis Exploratorio de Datos (EDA)

Este proyecto corresponde al Laboratorio 1 de la Especialización en Análisis de Datos.
El objetivo principal es aplicar un flujo end-to-end de análisis, desde la ingestión de datos hasta la formulación de conclusiones analíticas, utilizando herramientas del ecosistema Python.

 Objetivos del proyecto

Realizar el proceso ETL (Extracción, Transformación y Carga) sobre un conjunto de datos real.

Ejecutar un análisis exploratorio de datos (EDA) utilizando Python y pandas.

Formular tres preguntas de negocio basadas en los hallazgos del análisis.

Publicar la solución en GitHub con acceso directo al entorno Colab.

 Acceso al cuaderno en Google Colab

Podés abrir y ejecutar el análisis haciendo clic en el siguiente enlace:

🔗 Google Colab:
https://colab.research.google.com/drive/1NRSmIvWs1jU6NZWSHxqzF5ni3eu2W50T?usp=sharing

 Conjunto de datos

Fuente: Archivo local productos.csv

Descripción: Información de productos comercializados, incluyendo marca, presentación y precios.

 Columnas principales
Columna	Descripción
productos_descripcion	Nombre del producto
productos_marca	Marca del producto
productos_precio_lista	Precio base sin descuento
productos_precio_unitario_promo1	Precio con promoción aplicada
productos_cantidad_presentacion	Tamaño o cantidad de presentación
1. Proceso ETL
 Extracción

Se cargó el archivo CSV utilizando pandas:

import pandas as pd

df = pd.read_csv('/content/productos.csv', sep='|')

 Transformación

Se realizaron tareas de limpieza y estandarización como:

Ajuste de tipos de datos

Manejo de valores faltantes

Corrección de nombres y formato

Normalización de las variables de precio

Detalles completos disponibles en el cuaderno.

 Carga

Los datos transformados se mantuvieron en memoria para análisis posterior.
Opcionalmente pueden exportarse para su reutilización.

2. Análisis Exploratorio de Datos (EDA)

Se exploraron las características principales del dataset, incluyendo:

Distribución de precios

Comparación entre precio de lista y promocional

Presencia de marcas relevantes

Análisis de presentaciones y volumen

Identificación de outliers

Las visualizaciones se realizaron con:

pandas

matplotlib

seaborn (si aplica)

3. Preguntas de Negocio

Durante el proceso se formularon tres preguntas orientadas al negocio, tales como:

¿Qué marcas presentan mayor oferta de productos?

¿Cuál es la distribución de precios por marca?

¿Qué productos muestran la mayor diferencia entre precio base y promocional?

Las preguntas finales pueden variar según iteraciones del análisis.

 Requisitos

Python 3.9+

pandas

matplotlib

seaborn (opcional)

entorno Google Colab (recomendado)

 Resultados clave

Se preparó exitosamente el dataset para análisis.

Se desarrolló un EDA descriptivo que permitió identificar tendencias de precios y marcas.

Se plantearon 3 preguntas de negocio para interpretación y toma de decisiones.




