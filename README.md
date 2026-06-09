# BirdCLEF 2025 - Clasificación de audio multietiqueta

Este repositorio contiene los cuadernos desarrollados para el Trabajo de Fin de Grado centrado en la clasificación multietiqueta de audio dentro del reto BirdCLEF 2025. El objetivo principal es identificar la presencia de distintas especies de aves, anfibios, mamíferos e insectos a partir de grabaciones acústicas.

El proyecto trabaja con espectrogramas log-Mel generados a partir de señales de audio y modelos de redes neuronales convolucionales, incluyendo una CNN base y modelos preentrenados como EfficientNet-B0 y ResNet-18.

## Contenido del repositorio

### Cuadernos

`onthefly.ipynb`

Cuaderno principal de entrenamiento. Incluye la carga de metadatos, limpieza básica del dataset, preprocesamiento de audio, generación de espectrogramas log-Mel durante el entrenamiento y entrenamiento de los modelos.

`test_local.ipynb`

Cuaderno utilizado para evaluar los modelos sobre un subconjunto local separado del conjunto de entrenamiento. Su objetivo es obtener una referencia adicional del comportamiento del sistema antes de generar predicciones finales.

`inferencia.ipynb`

Cuaderno de inferencia utilizado para procesar los audios de test y generar el archivo `submission.csv` con el formato requerido por la competición.

## Entorno de ejecución

Los cuadernos fueron preparados y ejecutados principalmente en la plataforma Kaggle, por lo que algunas rutas siguen la estructura habitual de Kaggle, por ejemplo:

```text
/kaggle/input/
/kaggle/working/
