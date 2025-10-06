# Evaluación Módulo 3 – Exploración y Visualización de Datos

Este proyecto corresponde a la evaluación del Módulo 3 del bootcamp.  
El objetivo es limpiar y explorar dos datasets de clientes y vuelos, y responder a las 6 preguntas planteadas mediante visualizaciones.  
Se incluye además un bonus con una prueba de hipótesis (ANOVA) para analizar diferencias en vuelos reservados según el nivel educativo.

## Archivos incluidos
- `Evaluacion3.ipynb` → notebook principal con todo el análisis.
- `Customer Flight Activity.csv`
- `Customer Loyalty History.csv`

## Requisitos
- Python 3.x  
- Librerías: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`

## Ejecución
1. Colocar los CSV en la misma carpeta que el notebook.  
2. Abrir `Evaluacion3.ipynb` en Jupyter/VSCode.  
3. Ejecutar todas las celdas en orden.  

## Objetivo docente
Los objetivos de este módulo y de la presente evaluación son:  
- Python básico (funciones y conceptos del primer módulo).  
- Uso de Pandas.  
- Análisis exploratorio de datos (EDA).  
- Gestión de nulos.  
- Visualización de datos con matplotlib y seaborn.  
- Estadística descriptiva.  
- Estadística inferencial.  

## Notas metodológicas
- Primero se creó `df_flight_clean` tras depuración de datos.  
- Posteriormente se generó `df_flight_grouped` agrupando por `loyalty_number`, `year` y `month`.  
  - Esto convierte la clave primaria en compuesta (`loyalty_number`, `year`, `month`).  
  - Así cada fila representa la actividad de un cliente en un mes.  
  - El cambio de nombre a `df_flight_grouped` se hizo para diferenciarlo claramente del DataFrame original.  
- En las preguntas que requieren proporción de clientes (ej. tipo de tarjeta de fidelidad), se trabajó con un DataFrame reducido a **una fila por cliente** para evitar duplicaciones.  
- En gráficos categóricos se usaron barplots de medias, ya que los datos están agrupados y no es posible aplicar boxplots sobre distribuciones individuales.

## Retos encontrados
- Necesidad de agrupar por cliente, año y mes para definir correctamente la clave primaria.  
- Limitación de algunos gráficos de distribución (como boxplot) debido a que los datos estaban ya agregados.  
- Manejo de duplicados para no sobre-representar clientes con muchos vuelos.  
- El principal reto ha sido aplicar en un único proyecto toda la cantidad de conceptos vistos en este módulo en un tiempo limitado. Esto exigió priorizar claridad y sencillez.

## Autoría
Ela Ruiz González

