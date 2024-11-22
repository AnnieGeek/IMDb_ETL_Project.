# Carpeta Data 📂

Esta carpeta contiene los datos originales necesarios para ejecutar el pipeline ETL del proyecto.

## Contenido

1. **Archivo de Datos**
   - `movies_data.csv`: Archivo CSV que contiene información cruda sobre las películas extraída de IMDb, incluyendo:
     - Título
     - Año
     - Género
     - Duración
     - Calificación IMDb
     - Cantidad de votos
     - Director
     - Enlace a IMDb

## Notas

- Este archivo es el punto de partida para el proceso ETL y debe mantenerse en esta carpeta para que el pipeline funcione correctamente.
- Si deseas reemplazar este archivo por otro conjunto de datos, asegúrate de que el nuevo archivo siga el mismo formato y tenga el mismo nombre (`movies_data.csv`).
- El pipeline procesará este archivo para generar los datos transformados en la carpeta `output`.

