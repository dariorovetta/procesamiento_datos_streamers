
# Proyecto de Limpieza de Datos de Twitch

Este repositorio contiene notebooks de limpieza de datos específicos de un conjunto de datos de Twitch, enfocándose en filtrar y transformar la información para preparar los datos para análisis posteriores.

## Contenido del Repositorio

- **notebooks/limpiezaData.ipynb**: Notebook principal que realiza tareas de limpieza y filtrado de datos de un conjunto de datos de Twitch.

## Descripción de la Limpieza de Datos

Este notebook realiza los siguientes pasos de limpieza y preprocesamiento:

1. **Carga del Conjunto de Datos**:

   - Se carga el archivo `TwitchDataSet.csv` en un DataFrame de Pandas para manipular y analizar la información.
2. **Filtrado por Edad**:

   - Se filtran los registros donde el atributo `mature` es `False`, manteniendo solo los datos para menores de 18 años.
3. **Selección de Idiomas**:

   - Se identifican los idiomas más comunes y se crea una lista con los principales ocho idiomas (`English`, `Spanish`, `Korean`, `Russian`, `Portuguese`, `French`, `German`, `Italian`).
   - Se filtran los datos para mantener únicamente los registros en estos idiomas.
4. **Renombrado de Columnas**:

   - Las columnas se renombran para facilitar el análisis y mejorar la legibilidad, utilizando nombres más descriptivos en español, como `FOTO_PERFIL`, `CONTEO_SUPERIOR`, `NOMBRE_PANTALLA`, `TIEMPO_VISTA`, etc.
5. **Verificación de Tipos de Datos**:

   - Se verifica que los tipos de datos sean correctos y estén preparados para análisis posteriores.

## Datos

> **Nota Importante**:
> Los archivos de datos utilizados en este proyecto **no están incluidos en el repositorio** debido a su tamaño. Asegúrate de contar con el archivo `TwitchDataSet.csv` y colocarlo en la misma carpeta que el notebook o en una ruta accesible desde el notebook.

## Requisitos

Para ejecutar el notebook, se requieren las siguientes librerías de Python:

- `pandas`
- `numpy`
- `os` (incluido en la biblioteca estándar de Python)

Instala las librerías externas ejecutando:

```bash
pip install pandas numpy
```

## Ejecución

1. Clona este repositorio:
   ```bash
   git clone https://github.com/tu_usuario/tu_repositorio.git
   ```
2. Coloca el archivo `TwitchDataSet.csv` en la misma carpeta que el notebook o especifica su ruta dentro del código.
3. Abre y ejecuta el notebook `notebooks/limpiezaData.ipynb` para realizar la limpieza de datos.

## Contribuciones

Las contribuciones para mejorar el proceso de limpieza y optimizar el código son bienvenidas. Si deseas contribuir, realiza un fork del repositorio y abre un pull request con tus sugerencias.

## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.

---
