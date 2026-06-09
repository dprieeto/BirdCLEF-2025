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
```
Para ejecutarlos en otro entorno puede ser necesario adaptar las rutas de entrada, los datasets disponibles y los modelos preentrenados utilizados.

## Dataset

El proyecto se basa en el dataset de BirdCLEF 2025, compuesto por grabaciones de especies animales y metadatos asociados. Los audios originales no se incluyen en este repositorio debido a las condiciones de uso del dataset.

## Técnicas utilizadas

- Carga y preprocesamiento de audio.
- Filtro paso banda y normalización de la señal.
- Conversión a espectrogramas log-Mel.
- Entrenamiento on-the-fly.
- Clasificación multietiqueta.
- Modelos CNN, EfficientNet-B0 y ResNet-18.
- Agregación de predicciones por ventanas temporales.
- Generación de archivo `submission.csv`.

## Licencia

Este proyecto se publica bajo licencia MIT. Consulta el archivo `LICENSE` para más información.
