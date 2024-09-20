
💻 Proyecto de Regresión Logística: Predicción de Rendimiento de Cultivos

_Descripción del Proyecto_

Este proyecto tiene como objetivo predecir si el rendimiento de un cultivo será *Alto (1)* o *Bajo (0)* en función de tres variables independientes: la *cantidad de fertilizante usada*, la *calidad del suelo*, y la *cantidad de lluvia*. El análisis se realiza utilizando un modelo de *regresión logística*.

_Temática: Agricultura_

El proyecto analiza los datos de agricultura para determinar si las condiciones dadas de los cultivos afectarán positivamente o negativamente el rendimiento. La variable objetivo es el rendimiento del cultivo, donde:

- *0 = Bajo rendimiento (≤ 3000)*
- *1 = Alto rendimiento (> 3000)*

📌 _Objetivo_
El objetivo principal es predecir el rendimiento del cultivo basado en las características:
- **Cantidad de fertilizante usado**
- **Calidad del suelo**
- **Cantidad de lluvia**

Utilizamos un modelo de regresión logística para realizar esta predicción.


🏦 _Estructura del Proyecto_

- `Regresion_logistica.ipynb`: Contiene el código principal que implementa el modelo de regresión logística.
- `crop_production.csv`: (Opcional) Si tienes un archivo CSV con datos, este es el archivo que puedes utilizar para entrenar el modelo.
- `README.md`: Este archivo, que describe el propósito y los pasos para ejecutar el proyecto.


## Ejecución del Proyecto

1. *Clonar el repositorio*:
   
   Clona este repositorio en tu máquina local utilizando Git:
   
  git clone https://github.com/usuario/repo.git
  cd repo

3. *Cargar los datos*:
   
   Si tienes un archivo `crop_production.csv` con las variables necesarias (`FertilizerUsed`, `SoilQuality`, `Rainfall`, `CropYield`), asegúrate de que esté en el mismo directorio que el notebook.

4. *Abrir el notebook*:
   
   Abre el archivo `Regresion_logistica.ipynb` en _Google Colab_ o en tu entorno de Jupyter Notebook.

5. *Ejecutar el código*:
   
   Corre todas las celdas del notebook para entrenar el modelo de regresión logística con los datos de entrada.

------------------------------------------------

📄 _Descripción del Código_

El código se estructura de la siguiente manera:

1. *Importación de bibliotecas*:
   Se utilizan `pandas` para manipular los datos, `scikit-learn` para construir el modelo de regresión logística, y `matplotlib` para la visualización.

2. *Carga y preprocesamiento de datos*:
   Los datos se cargan en un `DataFrame` de pandas, y la variable objetivo `CropYield` se transforma en binaria: 
   - 0 = Bajo rendimiento (≤ 3000)
   - 1 = Alto rendimiento (> 3000)

3. *División de los datos*:
   El conjunto de datos se divide en conjunto de entrenamiento y de prueba (80% - 20%).

4. *Estandarización de las variables*:
   Las variables independientes (`FertilizerUsed`, `SoilQuality`, `Rainfall`) se estandarizan para asegurar que tengan la misma escala.

5. *Entrenamiento del modelo*:
   Se utiliza el modelo de regresión logística de `scikit-learn` para ajustar los datos de entrenamiento y realizar predicciones en los datos de prueba.

6. *Evaluación del modelo*:
   Se evalúa el rendimiento del modelo utilizando métricas como la exactitud, la matriz de confusión y el reporte de clasificación.

7. *Visualización*:
   Se incluye un gráfico que muestra cómo las diferentes variables afectan el rendimiento del cultivo.

------------------------------------------------

🎯 _Resultados Esperados_

Al ejecutar el modelo de regresión logística, deberías obtener resultados que muestren la exactitud del modelo y cómo las variables independientes influyen en el rendimiento del cultivo. Además, se genera una matriz de confusión y un reporte de clasificación con métricas como precisión, recall y F1-score.

------------------------------------------------

📢 _Contribuciones_

Si deseas contribuir a este proyecto, siéntete libre de hacer un **fork** y enviar un **pull request** con tus sugerencias o mejoras.
