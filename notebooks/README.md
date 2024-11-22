# Carpeta Notebooks 📓

Esta carpeta contiene el notebook principal del proyecto, que incluye todo el pipeline ETL y las visualizaciones generadas.

## Contenido

1. **Notebook Principal**:
   - `Peliculas.ipynb`: Este archivo incluye los siguientes procesos:
     - **Extracción de Datos**: Lectura del archivo CSV con las 250 películas mejor calificadas de IMDb.
     - **Transformación de Datos**:
       - Limpieza y normalización de las columnas.
       - Conversión de la duración de las películas a minutos y horas.
       - Clasificación de películas por décadas y calidad.
       - Enriquecimiento de datos con métricas calculadas.
     - **Carga de Datos**:
       - Exportación a un archivo CSV (`movies_transformed.csv`) en la carpeta `output`.
       - Almacenamiento en una base de datos SQLite (`movies.db`).
     - **Visualizaciones**:
       - Top 10 películas mejor calificadas.
       - Distribución de películas por décadas.
       - Relación entre votos y calificaciones IMDb.
       - Distribución de calificaciones IMDb.

## Notas

- Este notebook es el núcleo del proyecto y debe ejecutarse después de instalar todas las dependencias listadas en `requirements.txt`.
- Las salidas generadas por el notebook (gráficos, CSV, y base de datos) se almacenan en la carpeta `output/`.
- **Recomendación**: Revisa el entorno de Python antes de ejecutar este archivo, asegurándote de que todas las librerías necesarias estén instaladas.

---

### Cómo Ejecutar el Notebook

1. Asegúrate de que Jupyter Notebook esté instalado en tu máquina.
2. Ejecuta el siguiente comando en tu terminal:
   ```bash
   jupyter notebook notebooks/Peliculas.ipynb

3. Sigue las celdas del notebook paso a paso para ejecutar el pipeline ETL y generar las visualizaciones.
   
## Dependencias Principales
pandas: Manipulación de datos.
matplotlib: Visualización de datos.
sqlite3: Almacenamiento de datos en bases SQLite.




