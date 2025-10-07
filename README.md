# Evaluación Módulo 3 – Análisis de Vuelos y Clientes

Este proyecto corresponde a la **evaluación final del Módulo 3** del bootcamp de Data Analytics en Adalab.  
El objetivo es analizar el comportamiento de los clientes de una aerolínea, utilizando datos de vuelos y de su programa de fidelidad.

---

## Archivos incluidos

- `Evaluacion3.ipynb`: Notebook principal con todo el análisis paso a paso.
- `Customer Flight Activity.csv`: Dataset con información de la actividad de vuelos (número de vuelos, distancia, puntos acumulados, etc.).
- `Customer Loyalty History.csv`: Dataset con información de los clientes (salario, nivel educativo, estado civil, tipo de tarjeta de fidelidad, etc.).
- `README.md`: Este archivo de documentación.

---

## Contenido del análisis

1. **Pre-EDA y limpieza de datos**  
   - Revisión de nulos, duplicados y tipos de datos.  
   - Transformación de columnas temporales (año, mes) y creación de columna `date`.  
   - Consolidación de registros por cliente/año/mes.

2. **Análisis exploratorio (EDA)**  
   - Distribución de vuelos reservados a lo largo de los meses y años.  
   - Relación entre distancia y puntos acumulados.  
   - Distribución de clientes por provincia/estado.  
   - Análisis de salario medio por nivel educativo.  
   - Proporción de clientes por tipo de tarjeta de fidelidad.  
   - Distribución de clientes según estado civil y género.

3. **Estadística descriptiva e inferencial**  
   - Medidas de tendencia central (media, mediana, moda).  
   - Medidas de dispersión (desviación estándar, varianza).  
   - Intervalos de confianza para reservas de vuelos según nivel educativo.  
   - Pruebas de hipótesis para evaluar diferencias significativas entre grupos.

4. **Visualizaciones principales**  
   - Histogramas y boxplots para variables numéricas.  
   - Gráficas de barras y “pie charts” para categóricas.  
   - Scatterplots para relaciones numéricas.  
   - Heatmap de correlaciones.

---

## Conclusiones globales

- El **nivel educativo** no influye de manera significativa en el número de vuelos reservados.  
- El **tipo de tarjeta de fidelidad** muestra claras diferencias en la proporción de clientes.  
- El **estado civil y el género** también reflejan patrones en la distribución de clientes.  
- Factores como **tarjeta y características sociodemográficas** tienen más impacto que las variables académicas en el comportamiento de los clientes.

---

## Requisitos

El análisis fue realizado en Python 3. Se requiere instalar las librerías:

```bash
pip install pandas numpy matplotlib seaborn scipy
✍️ Autor: Ela Ruiz González
📅 Octubre 2025



