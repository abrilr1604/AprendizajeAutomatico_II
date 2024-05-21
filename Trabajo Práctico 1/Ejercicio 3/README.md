# Problema 3
## Descripción
En este problema, se proporciona un conjunto de datos que contiene imágenes de escenas naturales de todo el mundo. El objetivo es construir un modelo de clasificación utilizando redes neuronales convolucionales (CNN) para clasificar estas imágenes en una de las seis categorías predefinidas.

## Dataset
El dataset proporcionado contiene alrededor de 25,000 imágenes de tamaño 150x150, distribuidas en seis categorías:
- buildings
- forest
- glacier
- mountain
- sea
- street

## Objetivo
Utilizando el dataset proporcionado, el objetivo es construir y comparar el rendimiento de distintos modelos de clasificación de imágenes utilizando redes neuronales convolucionales y densas que puedan clasificar con precisión las imágenes de escenas naturales en una de las seis categorías mencionadas anteriormente.

Los modelos a diseñar son:
- Modelo con capas densas.
- Modelo con capas convolucionales y densas.
- Modelo que incluya bloques residuales.
- Modelo que utilice como backbone alguna de las arquitecturas disponibles en TensorFlow (transfer learning)

## Resultados
Se propuso entrenar todos los modelos bajo la misma cantidad de epocas (20) para así poder observar y comparar el entrenamiento y problemas de cada arquitectura propuesta. Además, se propuso una arquitectura adicional de redes convolucionales la cual cuenta con una profundidad más grande. El objetivo de esto es identificar el problema de estas en los gradientes descendientes desvanecientes en el entrenamiento vistos en el paper de ResNet, para poder gozar de un modelo más preciso por lo visto en el paper de VGGNet.

De esta manera, en el colab se explaya en la definición y entrenamiento de cada una

![image](https://github.com/abrilr1604/AprendizajeAutomatico_II/assets/109885056/bca02a58-e18e-4b1b-8fd1-3190cd29dbde)

Modelo 1: Red convolucional estándar. Modelo 2: Red convolucional profunda. Modelo 3: Red convolucional con bloques residuales.
Métricas y pérdida de cada modelo según las epocas de entrenamiento

Las mejores métricas se obtuvieron con la arquitectura de transfer learning, llegando a una accuracy del 91%.

## Instrucciones
Para poder acceder a las visualizaciónes de los modelos y el análisis exploratorio del dataset, dentro del directorio del problema 3 se encuentra el notebook de colab donde se realizó el trabajo.
