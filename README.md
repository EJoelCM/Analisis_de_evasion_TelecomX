# Análisis de Evasión de Clientes en Telecom X

Este proyecto realiza un análisis exploratorio de datos para identificar las causas principales de la evasión de clientes en la empresa Telecom X. El objetivo es proporcionar insights que ayuden al equipo de Data Science a desarrollar modelos predictivos y estrategias para reducir la tasa de abandono.

## Propósito del Análisis

El análisis busca entender qué factores influyen en la decisión de un cliente de dejar la empresa. Se explora la relación entre diversas características del cliente (demografía, servicios contratados, tipo de contrato, métodos de pago, etc.) y la probabilidad de que abandone el servicio.

## Estructura del Proyecto

El proyecto principal se encuentra en el notebook de Google Colab.

- `TelecomX_ETL.ipynb`: Contiene todo el código Python para la extracción, transformación, limpieza, análisis y visualización de los datos.
- `/content/`: Este directorio (dentro del entorno de Colab) almacena las imágenes generadas durante el análisis (`distribucion_churn_na.png`, `distribucion_churn.png`, `distribucion_evasion_categoricas.png`, `distribucion_evasion_numerica.png`).

## Ejemplos de Gráficos e Insights

El análisis ha revelado varias tendencias importantes en la evasión de clientes:

- **Distribución de Evasión General:** Alrededor del 26.6% de los clientes han evadido el servicio.

  ![Distribución de Evasión](https://raw.githubusercontent.com/EJoelCM/Analisis_de_evasion_TelecomX/refs/heads/main/graficas/distribucion_churn.png)

- **Factores Clave de Evasión:**
    - Los clientes con **Fibra Óptica** tienen una tasa de evasión más alta.
    - Los contratos **mes a mes** muestran una mayor tasa de abandono en comparación con contratos de mayor duración.
    - Los clientes con **cargos mensuales altos** y **contratos de corta duración** son más propensos a cancelar.

  Aquí tienes un ejemplo de la distribución de evasión en variables categóricas:

  ![Distribución de Evasión Categóricas](https://raw.githubusercontent.com/EJoelCM/Analisis_de_evasion_TelecomX/refs/heads/main/graficas/distribucion_evasion_categoricas.png)

  Y la distribución en variables numéricas:

  ![Distribución de Evasión Numéricas](https://raw.githubusercontent.com/EJoelCM/Analisis_de_evasion_TelecomX/refs/heads/main/graficas/distribucion_evasion_numerica.png)

## Instrucciones para Ejecutar el Notebook

1.  Abre el notebook en Google Colab.
2.  Asegúrate de tener conexión a internet para descargar los datos desde la URL proporcionada.
3.  Ejecuta cada celda del notebook secuencialmente.

El notebook realizará los siguientes pasos:
- Importación de librerías necesarias.
- Extracción de los datos desde la URL.
- Transformación y limpieza de los datos, manejando valores inconsistentes y mapeando variables categóricas a formatos numéricos.
- Análisis exploratorio de datos, incluyendo visualizaciones y cálculo de estadísticas descriptivas.
- Generación de gráficos de distribución de evasión.
- Cálculo de la matriz de correlación para identificar relaciones entre variables.

Al ejecutar el notebook, se mostrarán las visualizaciones y las tablas de análisis directamente en la salida de las celdas. Las imágenes clave también se guardarán en el directorio `/content/` dentro del entorno de Colab.
