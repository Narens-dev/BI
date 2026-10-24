# Proyecto de Business Intelligence - MoviBogotá S.A.

## Descripción del caso

MoviBogotá S.A. es un operador privado de transporte masivo urbano en Bogotá, responsable de más de 450 buses y más de 80 rutas. Actualmente, la organización padece una arquitectura accidental debido a la fragmentación de sus datos operativos (silos de datos en archivos planos, telemetría GPS e informes manuales de mantenimiento en Excel). Esto impide que la Gerencia de Operaciones y Planeación del Servicio tome decisiones oportunas para responder a la pregunta crítica del negocio:

> ¿Cómo programar y redistribuir de forma dinámica la flota de buses y las frecuencias de despacho por ruta e intervalos por horas, minimizando los costos de distancia recorrida en vacío y los tiempos de espera de los usuarios en estaciones de alta demanda?

El documento completo de la Entrega 1 está en [`docs/entregas/BI-Entrega-1-Equipo506232716.pdf`](docs/entregas/BI-Entrega-1-Equipo506232716.pdf).

## Integrantes

| Integrante | Código |
|---|---|
| David Santiago Prieto Beltrán | 506212024 |
| Naren Santiago Rojas Sánchez | 506232716 |
| Joseph David Vargas Olaya | 506232072 |

Docente: Leandro Pájaro Fuentes

## Herramientas

| Capa | Herramienta |
|---|---|
| Fuentes de datos | CSV y JSON (validaciones, Portal de Datos Abiertos, trazados y paraderos) |
| Integración (ETL) | Pentaho Data Integration (archivos `.ktr` y `.kjb`) |
| Almacén de datos | PostgreSQL (modelo en estrella) |
| Usuario final | Microsoft Power BI |
| Modelo predictivo | Python (notebooks) |
| Gobierno y versionamiento | GitHub, draw.io |

## Estructura del repositorio

```
├── README.md            caso, integrantes, herramientas y cómo reproducir
├── .gitignore
├── docs/
│   ├── entregas/        PDF de cada entrega (E1, E2, E3, final)
│   └── diagramas/       arquitectura y esquema dimensional: PNG + archivo editable (draw.io)
├── datos/
│   ├── raw/             fuentes originales
│   ├── muestras/        20 filas por fuente, en CSV
│   ├── diccionarios/    un diccionario por fuente
│   └── descarga.md      URL, fecha y pasos para obtener cada fuente
├── dw/
│   ├── ddl/             scripts CREATE TABLE de dimensiones y hechos
│   └── conciliacion/    consultas de conteo y totales por fuente
├── etl/
│   ├── transformaciones/  archivos .ktr de Pentaho
│   ├── trabajos/          archivos .kjb de Pentaho
│   └── README.md          orden de ejecución y parámetros
├── dashboard/           archivo .pbix o enlace publicado, y capturas
└── modelo/              notebooks de Python del modelo predictivo
```

## Cómo reproducir

1. Obtener las fuentes siguiendo [`datos/descarga.md`](datos/descarga.md); los archivos originales están en [`datos/raw/`](datos/raw/).
2. Revisar los diccionarios en [`datos/diccionarios/`](datos/diccionarios/) y los diagramas en [`docs/diagramas/`](docs/diagramas/). Los PNG se pueden arrastrar a [draw.io](https://app.diagrams.net/) para abrirlos como diagramas editables.
3. Los pasos de creación del data warehouse, ETL, dashboard y modelo predictivo se documentarán en las siguientes entregas.
