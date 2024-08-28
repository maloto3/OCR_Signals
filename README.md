# Trabajo_ReconocimientoTexto
Trabajo de la asignatura de Análisis de señales:

El objetivo es crear un OCR casero usando técnicas de análisis de señales. El esquema de funcionamiento de nuestro OCR es el siguiente:

1. Preprocesar la imágen usando dos técnicas diferentes:
    1.1 Algoritmo Canny para detectar los bordes de la imágen (las diferentes letras).
    1.2 Preprocesado con Wavelets para hallar el contraste entre fondo y letra

2. Segmentar la imágen preprocesada en las diferentes letras con el algoritmo Connected Components, implementado en la librería cv2.

3. Entrenar una red neuronal con el dataset EMNIST para la detección de letras (previamente escaladas y normalizadas para cuadrar formatos).
