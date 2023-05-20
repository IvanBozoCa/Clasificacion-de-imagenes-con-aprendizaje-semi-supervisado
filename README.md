# Clasificación de Imágenes usando Aprendizaje Semi-Supervisado

## Descripción

Este proyecto es una exploración práctica de cómo se puede utilizar el aprendizaje semi-supervisado, específicamente a través de un método conocido como self-training, para mejorar la eficiencia y precisión de los modelos de clasificación de imágenes.

El dataset utilizado es el FashionMNIST de TensorFlow, una colección de 60,000 imágenes de productos de moda. Este conjunto de datos se elige debido a su diversidad de categorías, lo que aporta un buen desafío para la clasificación de imágenes. La tarea de clasificación se lleva a cabo a través de un modelo de aprendizaje profundo construido con capas convolucionales, de agrupamiento, de aplanamiento y densamente conectadas.

Comenzamos el self-training con un conjunto de entrenamiento inicial de 20,000 imágenes y, en cada iteración, incorporamos las 500 imágenes con las predicciones más seguras (las de menor entropía) al conjunto de entrenamiento. La eficacia de este enfoque se mide a través del F1-Score, una métrica comúnmente utilizada para evaluar la precisión de los modelos de clasificación.

Además de evaluar la precisión del modelo, también estudiamos cómo la cantidad de datos y las iteraciones de self-training afectan al tiempo de entrenamiento. Los resultados de este estudio se presentan en forma de un informe detallado, que incluye gráficos del F1-Score y observaciones del rendimiento del modelo. El producto final es un buen clasificador, que distingue al menos datos obviamente distintos.

## Tecnologías Usadas

- Python
- TensorFlow
- Keras
- Matplotlib
- SciPy
- Scikit-learn
- NumPy

## Instalación

Es necesario tener instalado Visual Studio Code y Python. Las librerías necesarias se pueden instalar con pip:

