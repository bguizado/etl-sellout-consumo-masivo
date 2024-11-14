# ETL para Datos de Sell-Out en la Industria de Consumo Masivo

## 📈 Descripción
Este proyecto implementa un pipeline ETL que procesa datos de **sell-out** (ventas directas a consumidores) para una empresa del sector de **consumo masivo**. La solución abarca la extracción de datos en formato Excel proporcionado por el cliente, su transformación a formatos optimizados para análisis (CSV y Parquet), y la desnormalización para facilitar reportes y análisis de performance.

## 🛠️ Casos de Uso
- **Optimización del análisis de ventas**: Mejora la visibilidad de datos en tiempo real para los equipos de trade marketing.
- **Automatización de reportes**: Reducción del tiempo de generación de reportes periódicos de ventas.
- **Consolidación de datos de múltiples fuentes**: Facilita el análisis a nivel cliente y material.


## Situación actual

Dirección y Gerencia Comercial, realizan multiples consultas sobre el sell-out, esta data es procesada mediante power pivot y explorada en tablas dinamicas, lo cual funciono al inicio de la operación, debido a la baja cantidad de registros, esta solución no fue escalable en el tiempo

### Algunos problemas

- Manipular la data, tenía tiempos de ejecución de entre 30 minutos a mas.
- Saturación de la memoria RAM.
- Incumplimiento de deadlines de reportes de visualización.
- Insatisfación de los clientes internos y externos.

## Diagrama de flujo

Excel (Datos Crudos) 
   └──> CSV (Transformación con VBA)
        └──> Parquet (Optimización con Python)
             └──> Base de datos desnormalizada (3NF)
                  └──> Reporte final para análisis de ventas

