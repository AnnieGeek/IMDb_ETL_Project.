# Carpeta Output 📂

Esta carpeta contiene los resultados generados por el pipeline ETL, incluyendo los datos transformados y las visualizaciones creadas durante el análisis.

## Contenido

1. **Datos Transformados**
   - `movies_enriched.csv`: Archivo CSV que contiene los datos procesados, incluyendo:
     - Calificaciones IMDb
     - Votos convertidos a millones
     - Clasificación por década
     - Categorización de calificaciones (Alta, Media, Baja).
   - `movies.db`: Base de datos SQLite que almacena los datos enriquecidos para consultas y análisis avanzados.

2. **Visualizaciones**
   - `visualizations/`: Carpeta que incluye los gráficos generados, como:
     - `top_10_movies.png`: Gráfico de barras que muestra las 10 películas mejor calificadas.
     - `movies_by_decade.png`: Gráfico de barras que ilustra la distribución de películas por década.
     - `votes_vs_rating.png`: Gráfico de dispersión que relaciona los votos con las calificaciones IMDb.
     - `ratings_distribution.png`: Histograma que muestra la distribución de las calificaciones IMDb.



3. **Uso**

Los archivos en esta carpeta son generados automáticamente por el pipeline ETL. Si deseas analizar o utilizar estos datos:

1. **Para las visualizaciones**: Puedes abrir las imágenes directamente en cualquier visor.
2. **Para los datos procesados**:
3. **`movies_enriched.csv`**: Puedes abrirlo en Excel, Google Sheets o cualquier editor de texto.
4. **`movies.db`**: Utiliza un cliente SQLite (como DB Browser for SQLite) o conecta a la base de datos desde un script en Python con la biblioteca `sqlite3`.

---

## Notas

- Asegúrate de ejecutar correctamente el pipeline ETL para generar todos los archivos dentro de esta carpeta.
- Si modificas el pipeline, los datos y visualizaciones en esta carpeta serán reemplazado
- Los gráficos y los datos procesados son generados automáticamente al ejecutar el notebook principal (`Peliculas.ipynb`).
- Asegúrate de que esta carpeta exista antes de ejecutar el proyecto para evitar errores al guardar archivos.
- Puedes utilizar herramientas como Excel, Google Sheets o DB Browser for SQLite para explorar los datos contenidos en los archivos `.csv` o `.db`.

