# Predicción de Ataque al Corazón y Reconocimiento de Dígitos

## Propósito del Proyecto

Este proyecto tiene como objetivo aplicar técnicas de **Machine Learning** para dos tareas principales:

1. **Predicción de Ataque al Corazón**: Desarrollar un modelo capaz de predecir si un paciente tiene un alto riesgo de sufrir un ataque al corazón, basado en varios factores médicos.
   
2. **Reconocimiento de Dígitos Manuscritos**: Implementar un modelo para reconocer números dibujados a mano, utilizando imágenes capturadas desde una aplicación estándar como **Paint**.

El propósito principal es aplicar los conocimientos adquiridos en el uso de técnicas de **aprendizaje supervisado**, trabajando con modelos clásicos como **Regresión Logística**, **K-Nearest Neighbors (KNN)**, y **Árboles de Decisión**. Además, se lleva a cabo una evaluación detallada de cada modelo mediante métricas como la precisión, el recall, el F1-score y la matriz de confusión.

## Datos Utilizados

### 1. **Predicción de Ataque al Corazón**

Se utilizó un conjunto de datos de pacientes médicos que contiene características como la edad, el colesterol, la presión arterial, entre otras. La variable de salida es un valor binario que indica si el paciente ha tenido un ataque al corazón (1) o no (0).

**Columnas del conjunto de datos**:

- **Variables numéricas**: Edad, presión arterial, colesterol, etc.
- **Variables categóricas**: Sexo, tipo de dolor en el pecho, etc.
- **Variable objetivo**: `output` (1 = ataque al corazón, 0 = no ataque al corazón).

### 2. **Reconocimiento de Dígitos Manuscritos**

El conjunto de datos utilizado para esta tarea es **MNIST**, que contiene imágenes de dígitos manuscritos del 0 al 9. Cada imagen tiene un tamaño de 28x28 píxeles y está etiquetada con el número correspondiente.

## Técnicas Aplicadas

### 1. **Predicción de Ataque al Corazón**

Para la predicción de ataque al corazón se usaron los siguientes modelos:

- **Regresión Logística**: Un modelo básico y eficiente para clasificación binaria.
- **K-Nearest Neighbors (KNN)**: Un clasificador basado en la similitud de las instancias cercanas.
- **Árboles de Decisión**: Un modelo interpretativo que se usa para tomar decisiones en función de las características de los pacientes.
  
Se utilizó el **StandardScaler** para normalizar los datos numéricos y un **ColumnTransformer** para aplicar transformaciones a las columnas numéricas y categóricas de forma adecuada.

### 2. **Reconocimiento de Dígitos Manuscritos**

Para la predicción de los dígitos manuscritos, se aplicaron los siguientes pasos:

- **K-Nearest Neighbors (KNN)**: Este modelo se utilizó para clasificar los dígitos manuscritos en función de sus características (píxeles de la imagen).
  
Los resultados se evaluaron utilizando la **precisión**, la **matriz de confusión** y otras métricas de clasificación.

### Evaluación de Modelos

Para ambos conjuntos de datos, los modelos se evaluaron utilizando métricas estándar de clasificación:

- **Exactitud (Accuracy)**: Porcentaje de predicciones correctas.
- **Precisión (Precision)**: Proporción de verdaderos positivos sobre todos los positivos predichos.
- **Recall**: Proporción de verdaderos positivos sobre todos los positivos reales.
- **F1-Score**: Media armónica entre la precisión y el recall, utilizada como medida combinada.

## Resultados y Conclusiones

### 1. **Predicción de Ataque al Corazón**

El modelo de **Regresión Logística** mostró un rendimiento sólido para la predicción del riesgo de ataque al corazón. Tras aplicar la normalización y la codificación adecuada de las variables, se obtuvieron buenos resultados en términos de precisión, recall y F1-score.

- **Exactitud**: 90%
- **Precisión**: 93%
- **Recall**: 88%
- **F1-Score**: 90%

Se observó que la inclusión de características como la edad, el colesterol y la presión arterial mejora significativamente la capacidad predictiva del modelo.

### 2. **Reconocimiento de Dígitos Manuscritos**

El modelo de **K-Nearest Neighbors (KNN)** también mostró buenos resultados en el reconocimiento de dígitos manuscritos.

- **Exactitud con K=3**: 96.67%
- **Exactitud con K=14**: 95.67%

El modelo tiene una precisión excelente para reconocer dígitos escritos a mano, lo que demuestra que KNN es adecuado para tareas de clasificación de imágenes simples como esta.

### Conclusión Final

Este proyecto mostró cómo aplicar diversas técnicas de **aprendizaje supervisado** para abordar problemas reales, como la predicción de enfermedades y la clasificación de imágenes. Los modelos entrenados fueron efectivos tanto para la clasificación de riesgo de ataque al corazón como para el reconocimiento de dígitos manuscritos, demostrando la aplicabilidad de los métodos de **Regresión Logística** y **KNN** en distintos contextos.

## Resultados
![image](https://github.com/user-attachments/assets/326228a5-8426-4e37-879a-d274067ff500)
![image](https://github.com/user-attachments/assets/c7274ed0-6cfd-44f2-aba3-399b0602df2a)
![image](https://github.com/user-attachments/assets/a6a5a7b4-bf99-49d8-8d03-b8abd070345b)
![image](https://github.com/user-attachments/assets/694a5842-d471-4411-b239-32efbba06c81)
![image](https://github.com/user-attachments/assets/ddadd660-d143-4ab4-a584-7aff9d76601e)
