# Parte I Análisis de Préstamos Bancarios - Loan Prediction Benitez  Maria Laura

"Proyecto: Análisis de Préstamos Bancarios - Loan Prediction ".

Descripción del Proyecto

Este proyecto forma parte del curso de Ciencia de Datos en Coderhouse y tiene como objetivo analizar las características que afectan la aprobación de préstamos bancarios. Utilizaremos el Loan Prediction Dataset disponible en Kaggle, que incluye información demográfica y financiera de los solicitantes, junto con el estado de aprobación de los préstamos.

Abstract

El dataset  "Home Credit Default Risk" contiene datos de solicitudes de préstamos bancarios, con variables relevantes que incluyen ingresos del solicitante, ingresos del co-solicitante, historial crediticio, monto del préstamo y estado civil, entre otras. El objetivo de este análisis es identificar factores que puedan influir en la aprobación o rechazo de los préstamos y desarrollar un modelo predictivo que permita anticipar la probabilidad de incumplimiento en el pago del préstamo.

Este análisis permitirá a la institución mejorar sus políticas de evaluación crediticia, con un enfoque en la minimización del riesgo y la optimización de sus productos financieros.

Descripción del Dataset

El dataset contiene múltiples variables relacionadas con el perfil financiero y demográfico de los solicitantes de préstamos. Algunas variables clave incluyen:
AMT_INCOME_TOTAL: Ingreso total anual del solicitante.
AMT_CREDIT: Monto del crédito solicitado.
AMT_ANNUITY: Monto de la anualidad del préstamo.
NAME_CONTRACT_TYPE: Tipo de contrato (préstamo a corto o largo plazo).
DAYS_EMPLOYED: Días de empleo del solicitante.
TARGET: Variable objetivo que indica si el préstamo fue incumplido (1) o no (0).
Para este proyecto, emplearemos una versión reducida del dataset con aproximadamente 2000 filas, lo cual permite cumplir con los requisitos del proyecto y facilita el análisis y la presentación en GitHub.

Instrucciones para la Versión Completa del Dataset

Para quienes deseen trabajar con el dataset completo, pueden descargarlo directamente desde Kaggle siguiendo estos pasos:

Visita la página del dataset en Kaggle: Home Credit Default Risk Dataset.
Descarga el archivo application_train.csv.

Para usarlo en este proyecto, reemplaza el archivo application_train_reducido.csv con el dataset completo.
Archivos en el Repositorio

Este repositorio contiene los siguientes archivos:

application_train_reducido.csv: Versión reducida del dataset con 2000 filas, ideal para realizar el análisis básico y cumplir con los requisitos de la entrega.

train.csv y test.csv: Archivos iniciales utilizados como opciones potenciales para el proyecto. Estos datasets fueron evaluados, pero debido a sus limitaciones en tamaño, se decidió utilizar el Home Credit Default Risk Dataset como principal.

Objetivo del Proyecto
Identificar los factores que más influyen en la aprobación de un préstamo bancario y, a partir de estos, entender el perfil de riesgo de los solicitantes. Este análisis busca responder preguntas clave que ayuden a la institución financiera a optimizar sus criterios de evaluación y segmentación de clientes en el contexto de préstamos.

Preguntas de Interés
¿Qué características sociodemográficas están más asociadas con una alta tasa de aprobación de préstamos?
¿Existe una relación entre el ingreso mensual de los clientes y la probabilidad de aprobación del préstamo?
¿Cómo influye el historial crediticio en la decisión de otorgar un préstamo?
¿El monto solicitado y el ingreso del co-solicitante afectan la probabilidad de aprobación?

Hipótesis

Los solicitantes con ingresos más altos tienen una mayor probabilidad de aprobación de préstamos.
Un historial crediticio positivo aumenta la probabilidad de que un préstamo sea aprobado.
El monto del préstamo solicitado tiene una relación inversa con la probabilidad de aprobación, es decir, préstamos más altos son menos propensos a ser aprobados.
Los solicitantes casados o con co-solicitantes presentan una tasa de aprobación más alta debido a ingresos combinados.
Tipo de Vivienda y Estabilidad Financiera: Los solicitantes con propiedad de vivienda presentan un menor riesgo de incumplimiento.
Historial de Crédito: Un buen historial crediticio se asocia positivamente con la probabilidad de aprobación del préstamo.

Análisis y Visualización

El análisis se centrará en la exploración de datos, visualización de patrones y correlaciones entre variables, y la creación de un modelo predictivo que permita estimar la probabilidad de incumplimiento de un solicitante.

Estructura del Proyecto
Carga y limpieza de datos: Preparación del dataset para el análisis. Incluye la eliminación de valores nulos y el manejo de outliers.
Análisis Exploratorio (EDA): Realización de visualizaciones como Box Plot, Gráfico de Densidad, Diagrama de Dispersión, Histograma y Matriz de Correlación para explorar las relaciones entre las variables y observar patrones que impactan la aprobación de préstamos.

Formulación y Validación de Hipótesis: A partir de los insights obtenidos en el EDA, se validan las hipótesis propuestas.

Recomendaciones: Propuestas para mejorar las políticas de evaluación crediticia basadas en los hallazgos obtenidos en el análisis.

Requisitos Técnicos
Python: Utilizado para análisis y visualización de datos.
Pandas: Para la manipulación y análisis de datos.
Seaborn y Matplotlib: Para la creación de gráficos y visualizaciones.
Google Colab: Para ejecutar el análisis en un entorno de notebook.
GitHub: El proyecto y el dataset están alojados en un repositorio público de GitHub para facilitar la entrega y revisión.

Parte II: Recomendaciones y Propuesta de Modelo Predictivo

Descripción

En esta segunda entrega, profundicé en el análisis del dataset, formulando recomendaciones para la evaluación crediticia y proponiendo un modelo de predicción de incumplimiento.

Recomendaciones Basadas en el Análisis

Con base en el análisis exploratorio, recomiendo:

Evaluar ingresos y estabilidad laboral como factores de riesgo.
Considerar la antigüedad laboral y propiedad de bienes como indicadores de estabilidad financiera.
Incorporar puntuaciones externas de riesgo para refinar la precisión en la evaluación.

Propuesta de Modelo Predictivo: Random Forest

Se seleccionó Random Forest como modelo preliminar, dado que:

Maneja bien relaciones complejas y no lineales entre variables.
Permite interpretar la importancia de cada variable en el riesgo de incumplimiento.
Es fácil de implementar y ajustar en Python usando scikit-learn.

Variables Clave para el Modelo
El modelo utiliza variables como Ingreso_Total, Monto_Credito, Dias_Empleado, y Fuente_Externa para predecir el riesgo de incumplimiento.

Conclusión Parte I y II
La implementación de Random Forest ayudará a la institución a optimizar la evaluación de riesgo y segmentación de clientes en solicitudes de préstamos, permitiendo tomar decisiones informadas y minimizar riesgos financieros.  

Proyecto Final Evaluaciones y Conclusiones
Análisis de los Resultados Valores Nulos Las columnas Consultas_credito_anio y Consultas_credito_mes tienen valores nulos, pero han sido imputados correctamente para garantizar la integridad de los datos. Características Seleccionadas Las 5 mejores características seleccionadas según Chi-cuadrado son: Genero Cantidad_hijos Propietario_auto Propietario_inmueble Monto_credito Estas características han demostrado tener la mayor relación estadística con el objetivo (Riesgo_incumplimiento).

Modelos Evaluados Random Forest Entrenamiento:

Precisión y Cobertura: Altas para ambas clases (0 y 1), con valores de 97%-100%. Exactitud (accuracy): 99%, indicando que el modelo funciona excepcionalmente bien en el conjunto de entrenamiento. Matriz de Confusión: Clase 0: Todas las instancias correctas. Clase 1: Solo 33 instancias clasificadas incorrectamente. Prueba:

Precisión y Cobertura: Balanceadas en 90% para ambas clases. Exactitud (accuracy): 90%, un rendimiento sólido. Matriz de Confusión: Clase 0: 546 correctas, 54 incorrectas. Clase 1: 456 correctas, 56 incorrectas. Árbol de Decisión Entrenamiento:

Resultados idénticos a Random Forest, lo que indica que el modelo también generaliza bien en los datos de entrenamiento. Exactitud (accuracy): 99%. Prueba:

Resultados casi idénticos a Random Forest: Precisión y Cobertura: 90%-91%. Exactitud (accuracy)**: 90%. Optimización de Hiperparámetros Árbol de Decisión:

Mejores hiperparámetros: max_depth: Sin límite, lo que permite un ajuste completo del árbol a los datos. min_samples_leaf: 2, para evitar sobreajuste. min_samples_split: 2, indicando que no hay restricciones adicionales para dividir nodos. Random Forest:

Mejores hiperparámetros: max_depth: 10, limitando la profundidad del árbol para evitar sobreajuste. min_samples_split: 10, asegurando que las divisiones solo ocurran con suficientes datos. n_estimators: 100, utilizando 100 árboles para un promedio robusto. Conclusiones Comparación General:

Ambos modelos tienen un rendimiento prácticamente idéntico, con una ligera ventaja en interpretabilidad para el Árbol de Decisión. Random Forest podría ser preferible para escenarios donde la robustez y la resistencia a variaciones sean importantes. Hiperparámetros:

La optimización ajustó los modelos para evitar sobreajuste y mejorar la generalización, especialmente en el caso de Random Forest.

Haz doble clic (o ingresa) para editar

Resumen Ejecutivo
Contexto Comercial y Problema
En el sector financiero, la capacidad de predecir el riesgo de incumplimiento de los clientes es fundamental para optimizar las decisiones de crédito y reducir pérdidas financieras. Este proyecto analiza un conjunto de datos del sector bancario para identificar patrones en el comportamiento de los clientes y desarrollar modelos predictivos efectivos que puedan distinguir entre clientes que cumplen o incumplen con sus obligaciones crediticias.

Objetivo del Proyecto
Desarrollar un modelo de Machine Learning para predecir el riesgo de incumplimiento basado en características demográficas y financieras de los clientes. Los objetivos específicos incluyen:

Identificar las características más relevantes para la predicción del incumplimiento.
Implementar y evaluar modelos como Random Forest y Árbol de Decisión.
Generar visualizaciones que expliquen los resultados y guíen la toma de decisiones.
Procesos Realizados
Selección y Limpieza del Dataset:

Se seleccionó un dataset del sector bancario con más de 2000 filas y 15 columnas, que cumple con las especificaciones requeridas.
Se manejaron valores nulos en columnas clave como Consultas_credito_anio y Consultas_credito_mes, utilizando imputación con la mediana.
Se binarizó la variable objetivo Riesgo_incumplimiento para facilitar el modelado.
Selección de Características:

Utilizando el método de Chi-cuadrado, se identificaron las 5 características más relevantes:
Genero
Cantidad_hijos
Propietario_auto
Propietario_inmueble
Monto_credito
Análisis Exploratorio y Visualizaciones:

Se generaron gráficos de la importancia de características utilizando Random Forest.
Se visualizó el Árbol de Decisión para interpretar las reglas generadas por el modelo.

Modelado Predictivo:

Random Forest:
Precisión en prueba: 90%.
Mejores hiperparámetros: max_depth=10, min_samples_split=10, n_estimators=100.
Árbol de Decisión:
Precisión en prueba: 90%.
Mejores hiperparámetros: max_depth=None, min_samples_leaf=2, min_samples_split=2.
Ambos modelos mostraron un desempeño balanceado, con una ligera ventaja para Random Forest en estabilidad.
Manejo de Desbalanceo de Clases:

Se utilizó SMOTE para equilibrar la distribución entre clases, mejorando la capacidad de los modelos para identificar clientes incumplidores.
Resultados y Conclusiones
Modelos:

Ambos modelos alcanzaron una exactitud del 90% en el conjunto de prueba, con buenos indicadores de precisión y cobertura para ambas clases.
Random Forest ofrece mayor estabilidad, mientras que el Árbol de Decisión es más interpretable.
Impacto Comercial:

Las características seleccionadas permiten identificar patrones claros en los clientes, lo que facilita la segmentación y la toma de decisiones personalizadas.
El modelo puede integrarse en sistemas de gestión de riesgos para mejorar la predicción del incumplimiento y optimizar el proceso de aprobación de créditos.

Recomendaciones
Implementación:

Utilizar Random Forest en producción para garantizar estabilidad y robustez.
Complementar con Árboles de Decisión para generar reportes interpretables.
Próximos Pasos:

Ampliar el análisis con datos adicionales, como historial crediticio más detallado.
Optimizar aún más los modelos con técnicas avanzadas como Gradient Boosting o XGBoost.
Evaluar el impacto del modelo en el negocio mediante métricas financieras como reducción de pérdidas.
Documentación:

Incluir gráficos clave y explicaciones en los reportes para presentar los hallazgos a las partes interesadas.
Anexos
Visualización del Árbol de Decisión: Una representación gráfica de las reglas generadas por el Árbol de Decisión.

Gráficos de Importancia de Características: Comparación visual de las características más relevantes seleccionadas por Random Forest.

Conclusión de Proyecto Final
Con este trabajo, se ha construido un sistema predictivo confiable que permite a las instituciones financieras tomar decisiones informadas y reducir el riesgo asociado a los incumplimientos de crédito.



