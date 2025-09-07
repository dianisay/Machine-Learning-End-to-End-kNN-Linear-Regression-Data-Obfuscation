# Machine Learning End-to-End: kNN, Linear Regression & Data Obfuscation

Este proyecto demuestra un flujo completo de trabajo en Machine Learning, desde el preprocesamiento de datos hasta la evaluación de modelos, incorporando técnicas de clasificación, regresión y ofuscación de datos para preservar la privacidad sin perder capacidad predictiva.

## Objetivos del proyecto
- Preparar y limpiar datos para análisis y modelado.
- Evaluar el impacto del escalado y la métrica de distancia en k-Nearest Neighbors (kNN).
- Comparar kNN con un modelo base (dummy) en clasificación binaria.
- Implementar regresión lineal desde cero y con scikit-learn.
- Analizar el efecto (o ausencia de efecto) del escalado en regresión lineal.
- Aplicar ofuscación de datos mediante multiplicación por una matriz invertible y demostrar que no afecta las predicciones.
- Validar analíticamente y computacionalmente la invariancia de la regresión lineal ante la ofuscación.

## Contenido
1. **Preprocesamiento de datos**
   - Limpieza, renombrado de columnas y verificación de tipos.
   - Análisis descriptivo y detección de valores atípicos.
2. **Clasificación con kNN**
   - Comparación con y sin escalado (MaxAbsScaler).
   - Métricas: F1-score y matriz de confusión.
   - Comparación con modelo dummy.
3. **Regresión lineal**
   - Implementación propia usando álgebra lineal.
   - Comparación con scikit-learn.
   - Evaluación con RMSE y R².
4. **Ofuscación de datos**
   - Transformación de características con matriz invertible.
   - Recuperación de datos originales.
   - Demostración analítica y práctica de invariancia en regresión lineal.
5. **Conclusiones**
   - Resumen de hallazgos clave y buenas prácticas.

## Tecnologías y librerías
- Python 3.x
- NumPy, Pandas
- scikit-learn
- Seaborn, Matplotlib

## Resultados clave
- El escalado es crítico para kNN cuando las variables tienen rangos muy distintos.
- La métrica de distancia influye en la selección de vecinos, especialmente con datos escalados.
- En regresión lineal con solución analítica, el escalado no cambia las predicciones ni las métricas, pero sí la magnitud de los coeficientes.
- La ofuscación con matrices invertibles preserva exactamente las predicciones y métricas de la regresión lineal.

