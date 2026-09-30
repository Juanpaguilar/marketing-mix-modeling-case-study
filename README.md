# Caso de estudio: Marketing Mix Modeling aplicado (OLS → Ridge)

Notebook educativo que replica, paso a paso, la metodología estadística detrás de un modelo de **Marketing Mix Modeling (MMM)** con **Robyn (Meta)**, usando un dataset **simulado** de inversión semanal en Meta Ads, Google Ads, DV360 y TikTok, y su efecto en ventas.

> **Nota sobre los datos:** los proyectos reales de MMM en los que he trabajado están bajo acuerdo de confidencialidad con el cliente, por lo que este notebook usa datos 100% sintéticos generados para fines demostrativos. La metodología, las herramientas y el flujo de trabajo (exploración → detección de multicolinealidad → OLS → Ridge → interpretación de negocio → evaluación) sí reflejan el proceso real que apliqué en un proyecto de MMM con Robyn en un contexto de agencia de medios.

## Qué cubre el notebook

1. **Exploración de datos** — visualización de inversión por canal y detección de multicolinealidad (correlación y VIF).
2. **Regresión OLS** — ajuste de un modelo lineal clásico y por qué falla cuando los canales de medios se mueven juntos.
3. **Regresión Ridge** — cómo la regularización (el mismo principio que usa Robyn internamente) estabiliza los coeficientes frente a la multicolinealidad.
4. **Interpretación de negocio** — traducción de los coeficientes en contribución por canal y retorno relativo por peso invertido.
5. **Evaluación del modelo** — R² y análisis de residuos.

## Herramientas

Python · pandas · NumPy · statsmodels · scikit-learn (Ridge, RidgeCV) · matplotlib

## Cómo correrlo

1. Clona o descarga este repositorio.
2. Sube `caso_estudio_mmm.ipynb` y `caso_estudio_mmm.csv` a [Google Colab](https://colab.research.google.com/) (o ábrelo localmente con Jupyter), manteniendo ambos archivos en la misma carpeta.
3. Corre las celdas en orden — ya viene ejecutado con sus salidas y gráficos, pero puedes editarlo y experimentar con los parámetros.

## Contexto

Ingeniero Industrial especializado en Marketing Analytics y Performance Analytics. Más sobre mi experiencia en [LinkedIn](https://www.linkedin.com/in/juan-esteban-pab%C3%B3n-aguilar).
