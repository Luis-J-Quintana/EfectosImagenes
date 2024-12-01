# Filtros Paralelos en Imágenes

## Descripción del Proyecto
Este proyecto tiene como objetivo demostrar el uso de la **programación paralela** mediante la aplicación de múltiples filtros a un conjunto de imágenes. Utilizando técnicas de paralelismo (fino y grueso), se busca optimizar el procesamiento de imágenes, comparando los resultados y el rendimiento entre versiones secuenciales y paralelas.

## Características
- **Filtros Implementados**:
  - Escalado a niveles de gris.
  - Detección de bordes (filtro Sobel).
  - Suavizado (filtro Gaussiano).
- **Paralelismo**:
  - Paralelismo grueso: procesar imágenes completas por proceso.
  - Paralelismo fino: dividir cada imagen en bloques y aplicar filtros en paralelo.
- **Manejo de Memoria y Excepciones**:
  - Evitar problemas de concurrencia en acceso a memoria compartida.
  - Manejo de errores en procesos.

## Objetivos
1. Mostrar los beneficios de la programación paralela en el procesamiento de imágenes.
2. Comparar tiempos de ejecución entre las versiones secuenciales y paralelas.
3. Evaluar el **speedup** y la **eficiencia** del sistema.

## Tecnologías Utilizadas
- **Lenguaje**: Python 3.8+
- **Bibliotecas**:
  - `opencv-python`: Para el procesamiento de imágenes.
  - `multiprocessing`: Para la implementación de paralelismo.
  - `numpy`: Para operaciones matemáticas y de matrices.

## Requisitos del Sistema
1. Tener instalado Python 3.8 o superior.
2. Instalar las dependencias necesarias:
   ```bash
   pip install opencv-python numpy
