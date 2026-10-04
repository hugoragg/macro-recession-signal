# Semáforo de Recesión

Proyecto de la asignatura Desarrollo de Aplicaciones para la Visualización de Datos (DAVD), curso 2026-2027.
Autor: Hugo Raggini Paternain

## Descripción

Aplicación web interactiva que estima la probabilidad de que la economía de EE.UU. entre en recesión en los próximos 12 meses. Usa datos públicos de FRED (Reserva Federal de St. Louis) y un modelo de regresión logística, y muestra el resultado como un semáforo verde, ámbar o rojo, junto con su evolución histórica y las variables que lo explican.

El objetivo es acercar este tipo de información, que hoy suele estar en plataformas de pago o en formatos técnicos, a cualquier persona.

## Objetivos

- Construir un pipeline que descargue y procese automáticamente los datos de FRED.
- Entrenar un modelo explicable que estime la probabilidad de recesión a 12 meses.
- Desarrollar un dashboard interactivo con Dash y Plotly.
- Desplegar la aplicación en una URL pública.

## Datos

Fuente: FRED (https://fred.stlouisfed.org)

| Serie | Descripción |
|---|---|
| GS10, TB3MS | Bono a 10 años y letra a 3 meses (curva de tipos) |
| UNRATE | Tasa de paro |
| SAHMREALTIME | Regla de Sahm |
| USREC | Indicador oficial de recesión (variable objetivo) |

## Estructura prevista

    app.py              Aplicación Dash
    src/etl.py          Descarga y procesamiento de datos
    src/model.py        Modelo de predicción
    src/graphics.py     Gráficos
    requirements.txt
    Procfile
    render.yaml

## Plan de trabajo

| Fechas | Tarea |
|---|---|
| 5 oct | Propuesta, repositorio y README |
| 6 a 18 oct | Pipeline de datos y análisis exploratorio |
| 19 oct a 1 nov | Modelo y validación |
| 2 a 15 nov | Dashboard en Dash |
| 16 a 22 nov | Despliegue en Render |
| 23 a 26 nov | Ajustes finales y presentación |

## Uso de IA

Se ha utilizado Claude (Anthropic) como apoyo en la redacción de la propuesta, la definición del proyecto y la prueba inicial de datos.
