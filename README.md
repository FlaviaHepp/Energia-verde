# 🌱⚡Inteligencia de Energías Renovables: Predicción de Puntuación Verde 

Este repositorio contiene un proyecto integral de análisis, visualización y modelado predictivo del potencial de energía renovable, combinando datos de energía solar y eólica en grandes ciudades del mundo.

El objetivo es analizar patrones temporales y geográficos y predecir un Green Score, una métrica que resume la favorabilidad combinada de recursos renovables en cada momento y ubicación.

--

# 🎯Objetivos del proyecto

- Analizar datos horarios de energía solar y eólica.
- Comprender patrones diarios y geográficos de generación renovable.
- Comparar el potencial renovable entre ciudades globales.
- Explorar la relación entre radiación solar y velocidad del viento.
- Construir modelos de Machine Learning para predecir el Green Score.
- Evaluar modelos con métricas robustas y validación cruzada.
- Interpretar resultados mediante feature importance y SHAP values.
- Guardar modelos listos para inferencia.

--

# 🌍Contexto

A medida que el mundo avanza hacia economías de cero emisiones, evaluar el potencial renovable de los centros urbanos es clave para:
- Planificación energética
- Optimización industrial
- Infraestructura sostenible
- Sistemas híbridos solar–eólico

Este proyecto analiza datos de megaciudades globales para aportar evidencia cuantitativa a estas decisiones.

--

# 📁Dataset
- Archivo: global_green_energy_pulse_20260112.csv
- Frecuencia: Horaria
- Variables principales:
- shortwave_radiation (W/m²)
- wind_speed_100m (km/h)
- latitude, longitude
- city
- time
- green_score (variable objetivo)

--

# 🧹Limpieza y preparación de datos
- Verificación de valores faltantes y duplicados.
- Conversión de time a formato datetime.
- Extracción de features temporales: año, mes, día, hora
- Eliminación de columnas con data leakage.
- Detección automática de:
   - duplicados
   - valores faltantes
   - features problemáticas
- Escalado y codificación mediante pipelines.

--

# 🔍Análisis Exploratorio (EDA)
📊 Análisis temporal
- Radiación solar promedio por hora.
- Velocidad del viento promedio por hora.
- Identificación de horas óptimas para generación solar y eólica.

--

# 🏙️Análisis por ciudad
- Ranking de ciudades por Green Score promedio.
- Heatmaps de radiación solar por ciudad y hora.
- Comparación hemisférica y geográfica.

--

# 🔗Relaciones clave
- Solar vs. viento (complementariedad).
- Green Score vs. latitud.
- Distribución del Green Score (asimetría positiva).

--

# 📈Visualizaciones
- Line plots temporales
- Bar plots comparativos por ciudad
- Histogramas de Green Score
- Scatter plots multivariados
- Heatmaps horarios
- Matriz de correlación
- Gráficos interactivos con Plotly

--

# 🤖Modelado Predictivo
- Variable objetivo
- Green Score (regresión)
- Features utilizadas
- Radiación solar
- Velocidad del viento
- Latitud y longitud
- Hora del día

--

# 🧠Modelos entrenados
- Se comparan múltiples modelos:
- Linear Regression
- Random Forest
- Gradient Boosting
- XGBoost
- LightGBM
- Técnicas aplicadas:
   - Train/Test split
   - Feature scaling
   - One-Hot Encoding
   - Feature selection automática
- Validación cruzada K-Fold
- Comparación por R², MAE y MSE

--

# 📊Resultados
- Random Forest / Boosting models logran el mejor desempeño.
- Radiación solar y velocidad del viento son los predictores dominantes.
- El modelo muestra alta estabilidad en validación cruzada.
- El Green Score puede ser predicho con error bajo y buena generalización.

--

# 🔎Interpretabilidad
- Importancia de variables (feature importance).
- Análisis explicativo con SHAP values.
- Evaluación de residuos.
- Comparación Predicho vs. Real.

--

# 💾Persistencia y uso en producción
El proyecto guarda:
- Modelo entrenado
- Preprocesador
- Selector de features
- Incluye una función de inferencia:
  - predict(data)
- Lista para integrarse en sistemas productivos o APIs.

--

# 🛠️Tecnologías utilizadas
- Python
- pandas, numpy
- matplotlib, `seaborn`
- plotly
- scikit-learn
- xgboost, lightgbm
- shap
- `joblib`

--

# 🌱Insights clave
- La radiación solar sigue un ciclo diario muy marcado.
- El viento es más estable y complementa la energía solar.
- El potencial renovable varía significativamente entre ciudades.
- No existe una dependencia lineal fuerte entre viento y sol.
- Los sistemas híbridos maximizan la confiabilidad energética.
- El Green Score es predecible con alta precisión.

--

# 🚀Posibles extensiones
- Forecasting a 24/48 horas.
- Optimización de consumo industrial por horario.
- Dashboards en tiempo real.
- Integración con datos de demanda energética.
- API de predicción de Green Score.

--

👤Autor/a

Flavia Hepp
Data Science · Machine Learning · Energy Analytics · Sustainability
