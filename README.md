# Challenge-TelecomX

Análisis de Evasión de Clientes en TelecomX

Descripción General

Este proyecto analiza la evasión de clientes (churn) en TelecomX, una empresa con una alta tasa de abandono (26.54%). Usando Python, Pandas y Matplotlib en Google Colab, se realizó un proceso ETL y un análisis exploratorio de datos para identificar las causas del churn y proponer soluciones.

Problema

TelecomX tiene una tasa de churn del 26.54%, lo que significa que 1 de cada 4 clientes abandona la empresa. El objetivo es determinar las causas de esta alta tasa de evasión.

Datos
Fuente: TelecomX_Data.json

Columnas: Incluye customerID, Churn, tenure, Contract, Charges.Monthly, Charges.Total y servicios adicionales como OnlineSecurity y TechSupport.

Etapas de Ejecución del Código
Extracción: Se cargaron los datos JSON usando pd.read_json desde la URL proporcionada.

Transformación: Se desanidaron columnas anidadas, se manejaron nulos (por ejemplo, se imputó Charges.Total como 0 para tenure=0), se convirtió Churn a binario (Yes=1, No=0) y se aseguraron los tipos de datos correctos.

Carga: Se guardó el conjunto de datos limpio como TelecomX_Data_clean.csv.

Análisis Exploratorio: Se generaron estadísticas descriptivas, correlaciones y visualizaciones (histogramas, boxplots, gráficos de conteo) para identificar patrones de churn.

Informe Final: Se resumieron los hallazgos y se proporcionaron recomendaciones.

Archivos
TelecomX_LATAM.ipynb: Cuaderno Jupyter con el código completo.

TelecomX_Data_clean.csv: Conjunto de datos limpio.

Visualizaciones: Incluidas en el cuaderno (por ejemplo, distribución de tenure, churn por tipo de contrato).

Cómo Ejecutar
Abre TelecomX_LATAM.ipynb en Google Colab.

Ejecuta las celdas en orden para realizar el ETL, el análisis y ver los resultados.

Revisa el informe final en el cuaderno para obtener información detallada.

Dependencias
Python 3

Pandas

Matplotlib

Seaborn
