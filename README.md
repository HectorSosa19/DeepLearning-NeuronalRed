# Clasificación de Imágenes con CNN en el Conjunto de Datos CIFAR-10

Este proyecto implementa una red neuronal convolucional (CNN) en Python utilizando TensorFlow y Keras para clasificar imágenes en el conjunto de datos CIFAR-10. CIFAR-10 es un conjunto de datos estándar que contiene imágenes en color de 10 categorías diferentes, como aviones, automóviles, gatos, perros, etc.

## Descripción del Proyecto

El objetivo de este proyecto es construir y entrenar una CNN para clasificar imágenes en el conjunto de datos CIFAR-10. El modelo sigue una arquitectura de CNN clásica con capas convolucionales, de pooling, y densamente conectadas. Además, se incluyen visualizaciones del rendimiento durante el entrenamiento y una evaluación final de la precisión utilizando una matriz de confusión.

## Requisitos

Para ejecutar este proyecto, necesitas las siguientes bibliotecas de Python:

- `tensorflow`
- `matplotlib`
- `sklearn`
- `numpy`

Puedes instalar estas dependencias ejecutando:
```bash
pip install tensorflow matplotlib scikit-learn numpy
Estructura del Código
1. Importación de Librerías
El código comienza importando las bibliotecas necesarias para construir y entrenar el modelo de CNN, así como para visualizar los resultados y evaluar el rendimiento.

2. Definición de Tensores
Se muestra cómo definir tensores de varias dimensiones en TensorFlow, incluyendo un escalar, un vector y una matriz.

3. Cargar y Visualizar el Conjunto de Datos CIFAR-10
CIFAR-10 es cargado y una función (show_images) muestra una muestra de imágenes con sus respectivas etiquetas.

4. Preprocesamiento de Datos
Escalado: Las imágenes son escaladas para que los valores de los píxeles estén en el rango [0, 1].
Codificación One-Hot: Las etiquetas de clase se convierten a formato one-hot.
5. Configuración de la Arquitectura del Modelo
Una CNN secuencial es creada con:

Capas convolucionales (Conv2D) para extraer características,
Capas de pooling (MaxPooling2D) para reducir la dimensionalidad,
Capas completamente conectadas (Dense) para la clasificación final.
6. Configuración de Entrenamiento
El modelo es compilado utilizando el optimizador Adam, la función de pérdida de entropía cruzada categórica, y métricas como precisión y recall.

7. Entrenamiento del Modelo
El modelo se entrena en el conjunto de datos CIFAR-10. Se almacena el historial del entrenamiento para su análisis posterior.

8. Visualización del Rendimiento
La función show_performance_curve permite visualizar las curvas de rendimiento para la precisión y la precisión de validación, incluyendo el punto de intersección óptimo entre ambas curvas.

9. Evaluación del Modelo
El modelo realiza predicciones en el conjunto de prueba, y se calcula y muestra una matriz de confusión para analizar el rendimiento del modelo en cada clase.

Cómo Ejecutar el Proyecto
Clona este repositorio.
Asegúrate de tener instaladas las dependencias.
Ejecuta el archivo .py o el notebook en tu entorno de desarrollo.
Resultados Esperados
Curvas de rendimiento para precisión y precisión durante el entrenamiento y validación.
Una matriz de confusión que muestra el rendimiento en cada clase de CIFAR-10.
Contribuciones
Si deseas mejorar este proyecto, siéntete libre de crear un pull request o abrir un issue.

Créditos
Este proyecto utiliza CIFAR-10 y TensorFlow/Keras para demostrar una implementación básica de redes neuronales convolucionales.
