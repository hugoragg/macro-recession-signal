# Recession Traffic Light

Project for the course Desarrollo de Aplicaciones para la Visualización de Datos (DAVD), 2026-2027.
Author: Hugo Raggini Paternain

## Description

Interactive web app that estimates the probability of a US recession in the next 12 months. It uses public data from FRED (Federal Reserve Bank of St. Louis) and a logistic regression model, and shows the result as a green, amber or red traffic light, along with its historical evolution and the variables that drive it.

The goal is to make this kind of information, which today is mostly found in paid platforms or technical formats, accessible to anyone.

## Objectives

- Build a pipeline that automatically downloads and processes FRED data.
- Train an explainable model that estimates the 12-month recession probability.
- Develop an interactive dashboard with Dash and Plotly.
- Deploy the app at a public URL.

## Data

Source: FRED (https://fred.stlouisfed.org)

| Series | Description |
|---|---|
| GS10, TB3MS | 10-year Treasury and 3-month T-bill (yield curve) |
| UNRATE | Unemployment rate |
| SAHMREALTIME | Sahm rule indicator |
| USREC | Official recession indicator (target variable) |

## Planned structure

    app.py              Dash app
    src/etl.py          Data download and processing
    src/model.py        Prediction model
    src/graphics.py     Charts
    requirements.txt
    Procfile
    render.yaml

## Work plan

| Dates | Task |
|---|---|
| Oct 5 | Proposal, repository and README |
| Oct 6 to 18 | Data pipeline and exploratory analysis |
| Oct 19 to Nov 1 | Model and validation |
| Nov 2 to 15 | Dash dashboard |
| Nov 16 to 22 | Deployment on Render |
| Nov 23 to 26 | Final adjustments and presentation |
