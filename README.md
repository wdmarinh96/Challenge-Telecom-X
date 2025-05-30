# Challenge-Telecom-X
# Análisis de Evasión de Clientes (Churn) - Proyecto Telecomunicaciones

## Descripción del Proyecto

Este proyecto tiene como objetivo principal analizar el fenómeno de la evasión de clientes ("Churn") dentro de una empresa de telecomunicaciones. Utilizando un conjunto de datos proporcionado, se realiza un proceso de exploración y análisis para identificar los factores clave que influyen en la decisión de un cliente de cancelar su servicio.

El análisis descriptivo y exploratorio busca comprender las características de los clientes que evaden en comparación con los que permanecen, con el fin de obtener insights valiosos que puedan ser utilizados para estrategias de retención de clientes.

## Estructura del Proyecto

El proyecto consiste principalmente en un cuaderno de Google Colab (o Jupyter Notebook) donde se realiza todo el análisis. La estructura del cuaderno es la siguiente:

1.  **Introducción:** Presentación del problema de Churn y el objetivo del análisis.
2.  **Limpieza y Tratamiento de Datos:** Pasos para cargar, normalizar y limpiar el conjunto de datos.
3.  **Análisis Exploratorio de Datos (EDA):** Exploración de la distribución de la variable Churn y su relación con variables categóricas y numéricas, utilizando visualizaciones.
4.  **Conclusiones e Insights:** Resumen de los hallazgos clave del EDA.
5.  **Recomendaciones:** Sugerencias estratégicas basadas en los insights obtenidos.

## Conjunto de Datos

El análisis se basa en el conjunto de datos `TelecomX_Data.json`, disponible en la siguiente URL:
`https://raw.githubusercontent.com/ingridcristh/challenge2-data-science-LATAM/main/TelecomX_Data.json`

Este conjunto de datos contiene información sobre clientes de una empresa de telecomunicaciones, incluyendo sus servicios, contrato, información de cuenta y si han evadido o no.

## Requisitos y Dependencias

Para ejecutar este proyecto, necesitarás tener instalado Python y las siguientes librerías:

*   `pandas`: Para manipulación y análisis de datos.
*   `requests`: Para descargar el archivo JSON desde la URL.
*   `matplotlib`: Para crear visualizaciones estáticas.
*   `seaborn`: Para crear visualizaciones estadísticas más atractivas.
*   `IPython`: Específicamente para la función `display` si utilizas un entorno interactivo como Colab o Jupyter Notebooks.

Puedes instalar estas dependencias utilizando pip: bash pip install pandas requests matplotlib seaborn ipython
## Cómo Ejecutar el Proyecto

Este proyecto está diseñado para ser ejecutado en un entorno de cuaderno interactivo como **Google Colab** o **Jupyter Notebook**.

1.  Abre el archivo del cuaderno (`.ipynb`) en Google Colab o tu entorno Jupyter.
2.  Ejecuta las celdas de código en orden. El cuaderno está estructurado secuencialmente para realizar el proceso de análisis.

El código dentro del cuaderno se encargará de:

*   Descargar los datos directamente desde la URL.
*   Limpiar y preprocesar los datos.
*   Realizar el análisis exploratorio y generar visualizaciones.
*   Presentar las conclusiones y recomendaciones.

No es necesario ejecutar el código desde la línea de comandos como un script tradicional, aunque las operaciones básicas de pandas y matplotlib podrían adaptarse a ese formato si fuera necesario.

## Posibles Problemas y Soluciones

*   **KeyError en nombres de columnas:** Si obtienes un `KeyError` indicando que una columna no existe (`'TotalCharges'` en lugar de `'Charges.Total'`, `'MonthlyCharges'` en lugar de `'Charges.Monthly'`), verifica la ortografía y el uso de puntos en los nombres de las columnas después de la normalización. Consulta la salida de `df.columns` para confirmarlos.
*   **IndentationError:** Asegúrate de que las líneas de código estén correctamente indentadas en Python.
*   **FutureWarning (inplace=True):** Como se identificó durante el desarrollo, pandas está cambiando el comportamiento de `inplace=True` en algunas situaciones. Se recomienda utilizar la asignación directa (`df[col] = df[col].method(...)`) en lugar de `df[col].method(..., inplace=True)` para evitar advertencias futuras.

## Contribuciones

Las contribuciones son bienvenidas. Si encuentras alguna mejora o problema, por favor abre un 'issue' o envía un 'pull request' en el repositorio donde se aloje este código.

## Autor

[wdmarinh96]

