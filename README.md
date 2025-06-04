# Challenge-TelecomX
Análisis de Evasión de Clientes en TelecomX

Propósito del Análisis

El propósito de este análisis es identificar las causas del alto índice de evasión de clientes (churn) en TelecomX, que presenta una tasa de abandono del 26.54%. A través de un proceso ETL y un análisis exploratorio de datos, se buscan patrones que expliquen el churn y se proponen estrategias para reducirlo, utilizando Python, Pandas y Matplotlib en Google Colab.
Estructura del Proyecto y Organización de los Archivos
TelecomX_LATAM.ipynb: Cuaderno Jupyter que contiene el código completo, dividido en las siguientes secciones:
Extracción: Carga de datos desde el archivo JSON.

Transformación: Limpieza y desanidado de datos.

Carga: Generación del archivo limpio.

Análisis Exploratorio: Visualizaciones y estadísticas.

Informe Final: Resumen de hallazgos y recomendaciones.

TelecomX_Data_clean.csv: Archivo CSV con los datos limpios y transformados, listos para análisis (7,267 filas, 21 columnas).

Gráficos: Las visualizaciones están incluidas en el cuaderno (histogramas, boxplots, gráficos de conteo y matriz de correlación).

Ejemplos de Gráficos e Insights Obtenidos
Distribución de Tenure por Churn  
Gráfico: Histograma que muestra que los clientes con tenure < 10 meses tienen una alta probabilidad de churn, mientras que aquellos con más de 50 meses tienden a permanecer.  

Insight: Los clientes nuevos son más propensos a abandonar, lo que sugiere problemas de satisfacción inicial.

Churn por Tipo de Contrato  
Gráfico: Gráfico de conteo que indica que los contratos "Month-to-month" tienen un churn del 40%, frente a menos del 10% en contratos de 1 o 2 años.  

Insight: Los contratos a corto plazo facilitan la salida de clientes; se deben incentivar contratos largos.

Cargos Mensuales por Churn  
Gráfico: Boxplot que revela que los clientes que abandonan tienen una mediana de Charges.Monthly de ~$80, frente a ~$60 para los que se quedan.  

Insight: Los cargos mensuales altos están asociados con el churn, indicando sensibilidad al precio.

Churn por Servicios Adicionales (ejemplo: TechSupport)  
Gráfico: Gráfico de conteo que muestra un churn del 40% en clientes sin TechSupport, frente al 15% en los que sí lo tienen.  

Insight: La falta de servicios como TechSupport y OnlineSecurity aumenta el churn; estos servicios mejoran la lealtad.

Instrucciones para Ejecutar el Notebook
Abre el archivo TelecomX_LATAM.ipynb en Google Colab.

Asegúrate de tener instaladas las dependencias: Python 3, Pandas, Matplotlib y Seaborn (ya incluidas en Colab por defecto).

Ejecuta las celdas en orden para realizar el proceso ETL, el análisis exploratorio y visualizar los resultados.

Revisa el informe final al final del cuaderno para ver los hallazgos y recomendaciones detalladas.

Opcionalmente, descarga el archivo TelecomX_Data_clean.csv desde la pestaña de "Archivos" en Colab para trabajar con los datos limpios.
