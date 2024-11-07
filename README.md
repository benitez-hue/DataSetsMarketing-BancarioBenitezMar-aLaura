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

Conclusión
La implementación de Random Forest ayudará a la institución a optimizar la evaluación de riesgo y segmentación de clientes en solicitudes de préstamos, permitiendo tomar decisiones informadas y minimizar riesgos financieros.

