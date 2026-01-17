# Sales Data Analysis

## Descripción del Proyecto

Este proyecto contiene un análisis exhaustivo de datos de ventas semanales correspondiente a un período de 50 semanas (octubre 2012 - septiembre 2013). El análisis está implementado en un Jupyter Notebook que examina tendencias, cambios drásticos y patrones de compra según género y franja horaria.

## Preguntas de Investigación

El notebook aborda las siguientes preguntas analíticas:

1. **Visualización de ventas diarias** - Representación gráfica de las tendencias de ventas a lo largo de las 50 semanas
2. **Identificación de cambios drásticos** - Detección del momento en el que ocurren cambios significativos en el volumen de ventas
3. **Análisis estadístico** - Validación de significancia estadística mediante prueba t de Student (cálculo de p-valor)
4. **Análisis por género** - Investigación de cómo la proporción de compradores hombre vs mujer impacta en las ventas
5. **Segmentación horaria** - Distribución de ventas por franjas horarias del día (Noche, Mañana, Mediodía, Tarde)

## Datos

- **Fuente**: 50 archivos CSV con datos de ventas semanales
- **Período**: Octubre 2012 - Septiembre 2013
- **Columnas principales**:
  - `sale_time`: Timestamp de la transacción (formato: YYYY-MM-DD HH:MM:SS)
  - `purchaser_gender`: Género del comprador (male/female)

## Tecnologías Utilizadas

- **Python 3** - Lenguaje de programación
- **Jupyter Notebook** - Entorno interactivo para análisis
- **Pandas** - Manipulación y análisis de datos
- **Matplotlib** - Visualización de gráficos
- **SciPy** - Análisis estadístico (prueba t de Student)

## Resultados Principales

- **Cambio crítico detectado**: 29 de abril de 2013 con p-valor < 0.01 (altamente significativo)
- **Patrón horario**: El mediodía (12PM-6PM) concentra el 39.4% de las ventas
- **Mañana**: 30.8% de las ventas
- **Tarde**: 20.9% de las ventas
- **Noche**: 9.0% de las ventas

## Cómo Ejecutar el Notebook

### Requisitos Previos

```bash
pip install pandas matplotlib scipy jupyter
```

### Pasos para Ejecutar

1. Clonar este repositorio:
   ```bash
   git clone https://github.com/DemaAlejandro/sales-data-analysis.git
   cd sales-data-analysis
   ```

2. Instalar dependencias:
   ```bash
   pip install -r requirements.txt
   ```

3. Iniciar Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Abrir y ejecutar el archivo `salesDA.ipynb`:
   - Navega a `salesDA.ipynb` en la interfaz de Jupyter
   - Ejecuta las celdas secuencialmente usando `Shift + Enter`
   - Observa los gráficos y análisis estadísticos generados

## Estructura del Análisis

El notebook está organizado en las siguientes secciones:

1. **Importación de datos** - Carga de los 50 archivos CSV
2. **Limpieza y transformación** - Conversión de tipos de datos, agregación diaria
3. **Análisis de tendencias** - Visualización y detección de cambios
4. **Análisis estadístico** - Prueba t de Student para validar significancia
5. **Segmentación por género** - Análisis de proporciones de compra
6. **Análisis temporal** - Distribución de ventas por franja horaria

## Interpretación de Resultados

- La prueba t reveló una diferencia **altamente significativa** (p < 0.01) en las ventas antes y después del 29 de abril de 2013
- Este cambio no puede atribuirse únicamente a variaciones en la proporción hombre/mujer
- El patrón horario es consistente, con picos de compra en horas diurnas

## Notas Importantes

- Este repositorio fue creado automáticamente usando **MCP (Model Context Protocol) de GitHub en VSCode**
- Para reproducir los resultados, asegúrate de tener todos los archivos CSV en la carpeta `datasets/`
- Los gráficos se generan dinámicamente al ejecutar el notebook

## Licencia

Este proyecto está disponible bajo licencia MIT.

## Autor

Análisis realizado como parte del programa StrataScratch de Ciencia de Datos.

---

*Última actualización: Enero 2026*
