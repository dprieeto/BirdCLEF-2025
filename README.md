# BirdCLEF 2025 - Clasificación de audio multietiqueta

Este repositorio contiene los cuadernos desarrollados para el Trabajo de Fin de Grado centrado en la clasificación multietiqueta de audio dentro del reto BirdCLEF 2025. El objetivo principal es identificar la presencia de distintas especies de aves, anfibios, mamíferos e insectos a partir de grabaciones acústicas.

El proyecto trabaja con espectrogramas log-Mel generados a partir de señales de audio y modelos de redes neuronales convolucionales, incluyendo una CNN base y modelos preentrenados como EfficientNet-B0 y ResNet-18.

## Contenido del repositorio

```text
.
├── onthefly.ipynb        # Entrenamiento con generación de espectrogramas durante la ejecución
├── test_local.ipynb      # Evaluación sobre un conjunto de test local
├── inferencia.ipynb      # Generación de predicciones para el formato de submission
├── README.md
└── LICENSE
