# Análisis de Clientes y Vuelos – Evaluación Módulo 3
bda-modulo-3-evaluacion-final-marinarsd

## Descripción general

Esta evaluación forma parte del bootcamp de Data Analytics de Adalab y tiene como objetivo analizar el comportamiento de los clientes de un programa de fidelización de aerolíneas. Utilizando dos conjuntos de datos (información de vuelos y datos de clientes), se realiza una exploración, limpieza y visualización de los datos para extraer conclusiones relevantes.

---

## Objetivo del análisis

- Explorar posibles errores o inconsistencias en los datos.
- Unir ambos datasets de forma coherente.
- Analizar el comportamiento de los clientes según variables como educación, salario, género, tipo de tarjeta, vuelos y puntos acumulados.
- Visualizar las relaciones más relevantes entre las variables.

---

## Fuentes de datos

- `Customer Loyalty History.csv`: contiene información demográfica y de fidelización de los clientes.
- `Customer Flight Activity.csv`: contiene registros mensuales con vuelos y puntos acumulados por cliente.

---

## Pasos realizados

1. **Exploración inicial** de los dos datasets.
2. **Limpieza de datos**:
   - Imputación de valores nulos (`Salary`, `Cancellation Year/Month`).
   - Conversión de salarios negativos a positivos.
   - Creación de la columna `"Client Status"` (activo o cancelado).
3. **Unión de los datasets** por `"Loyalty Number"`.
4. **Visualizaciones**:
   - Vuelos por mes y año.
   - Relación entre distancia y puntos.
   - Salario medio por educación.
   - Proporción de tipos de tarjeta.
   - Distribución por estado civil y género.

---

## Principales hallazgos

- Fuerte correlación entre la distancia del vuelo y los puntos acumulados.
- El salario promedio aumenta con el nivel educativo.
- La mayoría de los clientes están casados, con distribución equilibrada por género.
- La tarjeta "Star" es la más común entre los clientes.
- Muchos registros muestran meses sin vuelos aunque los clientes están activos (filtrado por `"Total Flights"` ayuda a limpiar los datos).

---

## Herramientas utilizadas

- Python 3
- pandas
- seaborn
- matplotlib
- Jupyter Notebook (usado en Visual Studio Code)

---

## Cómo ejecutar el análisis

1. Abre el archivo `.ipynb` (notebook) en Jupyter o VS Code.
2. Asegúrate de tener instaladas las librerías necesarias (`pandas`, `matplotlib`, `seaborn`).
3. Ejecuta las celdas paso a paso para ver la limpieza, unión y visualización de datos.

