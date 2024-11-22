# 🎬 IMDb ETL Project

Pipeline ETL para análisis de datos de IMDb con Python. Este proyecto muestra cómo extraer, transformar y cargar datos para obtener insights sobre las 250 películas mejor calificadas según IMDb.

---

## 📋 Estructura del Proyecto

El repositorio tiene la siguiente estructura:
IMDb_ETL_Project/ ├── data/ │ └── imdb_top_250.csv # Archivo con los datos originales ├── notebooks/ │ └── Peliculas.ipynb # Notebook Jupyter con todo el pipeline ETL ├── output/ │ ├── movies_transformed.csv # Datos transformados en formato CSV │ ├── visualizations/ # Carpeta para gráficos generados │ ├── top_10_movies.png # Visualización del Top 10 │ ├── movies_by_decade.png # Distribución por décadas │ └── movie_ratings_vs_votes.png # Relación entre calificación y votos ├── README.md # Descripción del proyecto ├── requirements.txt # Dependencias del proyecto


---

## 📊 Descripción del Pipeline ETL

### **1. Extract (Extracción):**
- Los datos fueron extraídos desde el archivo `imdb_top_250.csv` proporcionado en la carpeta `data/`.

### **2. Transform (Transformación):**
- Limpieza de datos:
  - Eliminación de duplicados.
  - Conversión de la columna `Duration` a minutos y horas.
- Enriquecimiento de datos:
  - Clasificación por **décadas**.
  - Categorización de **calidad de películas** basada en su calificación IMDb.
  - Conversión de votos a un formato más legible (en millones).

### **3. Load (Carga):**
- Los datos transformados se almacenaron en:
  - `movies_transformed.csv` en la carpeta `output/`.
  - Una base de datos SQLite para facilitar consultas.

---

## 📈 Visualizaciones

Se generaron las siguientes visualizaciones:
1. **Top 10 películas mejor calificadas**:
   - Archivo: `output/visualizations/top_10_movies.png`
   - Muestra las 10 películas con mejores calificaciones en IMDb.

2. **Distribución de películas por década**:
   - Archivo: `output/visualizations/movies_by_decade.png`
   - Analiza cuántas películas por década forman parte del Top 250.

3. **Relación entre calificaciones IMDb y votos**:
   - Archivo: `output/visualizations/movie_ratings_vs_votes.png`
   - Explora la relación entre las calificaciones y la popularidad (medida por número de votos).

---

## 🛠️ Herramientas Utilizadas

### **Librerías de Python:**
- `pandas`: Procesamiento y manipulación de datos.
- `matplotlib`: Creación de gráficos y visualizaciones.
- `sqlite3`: Manejo de bases de datos SQLite.

### **Entorno:**
- **Jupyter Notebook**: Desarrollo del pipeline ETL.
- **GitHub**: Documentación y versionado del proyecto.

---

## 🖥️ Cómo Ejecutar el Proyecto

1. Clona este repositorio:
   git clone https://github.com/<TU_USUARIO>/IMDb_ETL_Project.git
   cd IMDb_ETL_Project
   
2.Instala las dependencias:
pip install -r requirements.txt

3. Abre el archivo Jupyter Notebook:
jupyter notebook notebooks/Peliculas.ipynb

4.Explora los resultados en las carpetas output/ y visualizations/.

---

## 🤔 Conclusiones
Calificaciones Altas: Existe una correlación entre la cantidad de votos y las mejores calificaciones en IMDb.
Predominancia Histórica: Las décadas de los 1990 y 2000 tienen mayor representación en el Top 250.
Directores Destacados: Christopher Nolan y Steven Spielberg figuran como los directores con más películas en el Top 10.



