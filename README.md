# Modelo lineal para la puntuación IMDb

**Proyecto académico de análisis estadístico en R**

**Autoras:** Valentina Rodríguez Blanco, Macarena Perdomo y Sol Astengo.

## Descripción

El proyecto estudia la asociación entre la puntuación de películas en IMDb y distintas características, entre ellas el año de estreno, la cantidad de votos, los géneros, la certificación y variables relacionadas con su contenido. Se ajusta un modelo de regresión lineal múltiple y se evalúan sus supuestos, la inferencia sobre los coeficientes y su desempeño predictivo.

El conjunto de datos contiene inicialmente **4.227 películas**. Después de la depuración descrita en el informe, el análisis utiliza **3.931 observaciones**.

## Metodología

- Preparación de datos y tratamiento de valores faltantes.
- Ajuste de modelos de regresión lineal múltiple en R.
- Diagnóstico de multicolinealidad, linealidad, heterocedasticidad y normalidad de residuos.
- Identificación de observaciones atípicas y potencialmente influyentes.
- Inferencia sobre coeficientes, incluyendo el uso de errores estándar robustos HC3.
- Evaluación predictiva mediante 1.000 particiones aleatorias de entrenamiento (80 %) y prueba (20 %).

## Resultados informados

El modelo final presentado en el informe tiene un **R² de 0,4219** y un **R² ajustado de 0,4185**. El informe también presenta el comportamiento de una medida de desempeño calculada sobre las particiones de entrenamiento y prueba. Los resultados y sus interpretaciones se pueden consultar en el PDF original.

## Tecnologías

- **R** para procesamiento de datos, regresión, diagnóstico e inferencia.
- **Quarto** para la elaboración del informe reproducible.
- Bibliotecas de R, entre ellas `ggplot2`, `dplyr`, `readxl`, `car`, `lmtest` y `sandwich`.

## Archivos

- [`ProyectoIMBd.pdf`](ProyectoIMBd.pdf): informe académico final.
- [`proyecto.qmd`](proyecto.qmd): archivo fuente de Quarto.
- [`imdb_datos_limpios.xlsx`](imdb_datos_limpios.xlsx): conjunto de datos utilizado por el código.

> **Nota de ejecución:** el archivo `.qmd` lee los datos desde `imdb_datos_limpios.xlsx`. Para ejecutar el código sin modificar el original, el archivo de datos debe tener exactamente ese nombre y estar en el directorio de trabajo correspondiente. La reproducción también requiere instalar las bibliotecas utilizadas en el documento. La ejecución completa no ha sido verificada en este repositorio.

## Contexto y autoría

Este proyecto fue realizado en equipo como trabajo académico y se conserva en su versión original aprobada. La publicación documenta esa entrega, sin presentar cambios posteriores como parte del trabajo evaluado.
