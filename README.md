# Análisis y Predicción de Default de Préstamos Bancarios

## Descripción del Dataset

- **Nombre:** Loan Default Dataset
- **Fuente:** [Kaggle - Loan Default Dataset](https://www.kaggle.com/datasets/yasserh/loan-default-dataset)
- **Tamaño:** 148,670 registros y 34 variables
- **Variable Objetivo:** `status` (0 = Pagado, 1 = Impago)
- **Tipo de Tarea:** Clasificación Binaria

## Metodología Resumida

1. **EDA:** Análisis de nulos, outliers, balance de clases y correlaciones.
2. **Preprocesamiento:** Pipeline con imputación (mediana/moda) y escalado (RobustScaler).
3. **PCA:** Reducción a 34 componentes (90% de varianza explicada).
4. **Clustering:** K-Means con K=2 (Silhouette Score: 0.9426).
5. **Modelado:** Regresión Logística y Random Forest con GridSearchCV.
6. **Evaluación:** Métricas de clasificación y curvas ROC.

## Resultados del Mejor Modelo

| Métrica | Valor |
|---------|-------|
| **Modelo** | Random Forest |
| **Accuracy** | 0.9995 |
| **F1-Score** | 0.9990 |
| **ROC-AUC** | 1.0000 |
| **Tiempo de entrenamiento** | 1426.2 segundos |

✅ **Random Forest fue seleccionado como el mejor modelo por su rendimiento superior.**

## Video de Presentación

[Enlace al video](https://youtu.be/TU_ENLACE_AQUI)

## Cómo Reproducir el Análisis

```bash
# Clonar el repositorio
git clone https://github.com/jriosecobarahona-debug/loan-default-prediction.git

# Instalar dependencias
pip install -r requirements.txt

# Abrir el notebook en Jupyter o Colab
