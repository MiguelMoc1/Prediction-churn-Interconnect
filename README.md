# 📉 Predicción de Cancelación de Clientes (Churn) - Interconnect 🛠️

Bienvenido al repositorio de uno de mis proyectos más destacados: **Predicción de Churn** para la empresa ficticia **Interconnect**, en donde apliqué técnicas avanzadas de análisis de datos y machine learning para resolver un problema clave en el sector de telecomunicaciones: **identificar clientes propensos a cancelar su servicio**. Este proyecto no solo ayuda a retener clientes, sino que también ofrece insights valiosos para diseñar estrategias personalizadas de fidelización.

---

## 🔍 Resumen del Proyecto

El objetivo principal fue construir un modelo de machine learning que predijera con precisión si un cliente cancelaría su servicio. Para lograr esto, trabajé con datos de:
- **Contratos** (tipo de contrato, método de pago, etc.).
- **Datos personales** (género, si es ciudadano senior, etc.).
- **Servicios** de internet y teléfono.

### 🚀 Proceso de Desarrollo
1. **Análisis Exploratorio de Datos (EDA):**
   - Identificación de patrones entre las características y la cancelación.
   - Visualización de datos y detección de anomalías.
2. **Preprocesamiento:**
   - Imputación de valores nulos en columnas críticas.
   - Codificación de variables categóricas con técnicas como One-Hot Encoding.
   - Generación de nuevas características para enriquecer los datos.
   - Balanceo de datos mediante sobremuestreo.
3. **Modelado:**
   - Entrenamiento y evaluación de **Regresión Logística**, **Árbol de Decisión** y **Bosque Aleatorio**.
   - Optimización de hiperparámetros con **GridSearchCV**.
4. **Resultados y Selección de Modelo:**
   - Selección del **Bosque Aleatorio** como modelo final por su excelente balance entre precisión y sensibilidad.

---

## 🛠️ Herramientas y Tecnologías

- **Lenguajes:** Python.
- **Librerías Principales:** 
  - `pandas`, `numpy` para manipulación de datos.
  - `matplotlib`, `seaborn` para visualización de datos.
  - `scikit-learn` para el modelado y preprocesamiento.
- **Técnicas Adicionales:**
  - Sobremuestreo de datos desbalanceados con `resample`.
  - Optimización con `GridSearchCV`.

---

## 📈 Principales Resultados

| Modelo                | AUC-ROC (Test) | F1-Score (Test) |
|-----------------------|----------------|-----------------|
| **Random Forest**     | 0.840          | 0.633           |
| Logistic Regression   | 0.828          | 0.604           |
| Decision Tree         | 0.834          | 0.627           |

El modelo **Random Forest** fue elegido como el modelo final debido a su:
- Excelente desempeño en el conjunto de prueba.
- Robustez frente a datos complejos y desbalanceados.

---

## 🎯 Conclusiones y Recomendaciones

1. **Conclusiones Clave:**
   - Los clientes con servicios de fibra óptica tienen una mayor tasa de cancelación.
   - Cargos mensuales altos son un factor importante en la cancelación.
   - El modelo final (Random Forest) permite identificar clientes en riesgo con gran precisión.

2. **Recomendaciones para la Empresa:**
   - Ofrecer descuentos personalizados a clientes con altas probabilidades de cancelación.
   - Mejorar la percepción de valor en los servicios de fibra óptica.
   - Usar las predicciones del modelo para priorizar campañas de fidelización.

---
