# Clasificador de Galaxias

El trabajo es desarollado en el marco de una actividad de Extensión-Educación por parte de la Iniciativa de Datos e Inteligencia Artifical (IDIA) de la Universidad de Chile en conjunto con el Junior Achivement Chile para estudiantes de Media vocacional.


## Introducción
Edwin Hubble (XXXXX) desarrollo un esquema de clasificacipon de galaxias basado en su morfología (Referencia). En grandes rasgos se pueden classificar en Galaxías Elipticas (E), Galaxias Espirales (S) y Galaxias Irregulares (Irr), como se puede ver en la figura XXX [^1]. Con el objetivo más general de poder desarrollar un classificador más preciso la Universidad YYYYY desarollo un proyecto de ciencia ciuddadana conocido como Galaxy Zoo (Referencia) en el cual miles de voluntarios han venido clasificando imagenes de galaxias obtenidas por el Sloan Digital Sky Survey (SDSS) segun su morfología. De manera que podemos valernos de este dataset oara entrenar modelos de Deep Learning para la clasificación automática de galaxias.

## Objetivos 
- Entrenar un modelo sencillo de Deep Learning para la clasificación de imagenes de Galaxías en sus diferentes morfologias generales segun la clasificación de Hubble.

## Metodología
Usando el dataset de Galaxy Zoo entreremos un modelo de classificación de imanges basado en una red neuronal convolucional (CNN). El dataset cuenta con imágenes de galaxias clasificadas en las tres categorías principales: Elípticas, Espirales e Irregulares. Usaremos técnicas de preprocesamiento de imágenes, como el escalado y la normalización, para preparar los datos para el entrenamiento del modelo. Luego, construiremos una CNN utilizando una biblioteca de deep learning como PyTorch. El modelo será entrenado y evaluado utilizando métricas como la precisión, la recuperación y la F1-score para asegurar un rendimiento adecuado. Para obtener los datos utlizaremos la plataforma Kaggle, donde se encuentra disponible el dataset de Galaxy Zoo.

Una imagen ilustrativa del classificador se muestra en la figura XXX.

La loss function a utilizar será Cross Entropy Loss, adecuada para problemas de clasificación multiclase. El optimizador seleccionado será Adam, conocido por su eficiencia y capacidad para manejar grandes conjuntos de datos y parámetros.

Cómo la idea es que los estudiantes puedan entender y modificar el código, se utilizará una arquitectura CNN sencilla con pocas capas convolucionales y de pooling, seguida de capas completamente conectadas. Esto permitirá a los estudiantes observar cómo cada componente contribuye al rendimiento del modelo sin abrumarlos con complejidades innecesarias. Se usará un notebook de Jupyter para facilitar la interacción y visualización de resultados durante el proceso de desarrollo y entrenamiento del modelo.

[^1]: Para nuestra actividad inicial las subclases de cada uno de estas clases se escapa más alla de lo que busca esta actividad introductoría del uso de Inteligencia Artifical aplicada a astronomía.

## Resultados

Una imagen representativa de cada una de las clases de galaxias a clasificar se muestra en la figura XXX.

Una vez entrenado el modelo, se evaluará su rendimiento utilizando un conjunto de datos de prueba separado. Se calcularán métricas como la precisión, la recuperación y la F1-score para cada clase de galaxia (Elípticas, Espirales e Irregulares). Además, se generará una matriz de confusión para visualizar el desempeño del modelo en la clasificación de las diferentes morfologías galácticas. Los resultados obtenidos serán comparados con estudios previos para validar la efectividad del modelo desarrollado.


## Referencias

- Sreejith, S., Pereverzyev, S., Jr., Kelvin, L. S., Marleau, F. R., Haltmeier, M., Ebner, J., Bland-Hawthorn, J., Driver, S. P., Graham, A. W., Holwerda, B. W., Hopkins, A. M., Liske, J., Loveday, J., Moffett, A. J., Pimbblet, K. A., Taylor, E. N., Wang, L., & Wright, A. H. (2018). Galaxy And Mass Assembly: Automatic morphological classification of galaxies using statistical learning. Monthly Notices of the Royal Astronomical Society, 474(4), 5232–5258. https://doi.org/10.1093/mnras/stx2976

- Simonyan, K., & Zisserman, A. (2015). Very deep convolutional networks for large-scale image recognition. arXiv. https://arxiv.org/abs/1409.1556

## Autor
Steve Jurado [@jurados](https://github.com/jurados)
sjurado@das.uchile.cl

Fecha: 11/2025

