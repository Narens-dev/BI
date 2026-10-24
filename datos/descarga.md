# Guía de Descarga y Obtención de Fuentes - MoviBogotá S.A.

Este documento detalla la procedencia, los enlaces oficiales, las fechas de descarga y los pasos necesarios para obtener las fuentes de datos utilizadas en la Fase 1 del proyecto.

## 1. Fuente F1: Registro Transaccional de Validaciones

* **Descripción:** Datos transaccionales y de validaciones de pasajeros del sistema de transporte urbano.
* **Formato:** CSV (`Dataset_registros.csv`).
* **Volumen:** 55.000 registros.
* **Periodo:** Enero 2024 - Diciembre 2025.
* **Fecha de descarga / generación:** 20/10/2026.
* **Procedencia y pasos:**
  - Archivo sintético generado institucionalmente para complementar la simulación operativa de la flota ante la falta de apertura de datos crudos en tiempo real.
  - Se encuentra almacenado directamente en la ruta [`/datos/raw/Dataset_registros.csv`](raw/Dataset_registros.csv).

## 2. Fuente F2: Catálogo Zonal y Estaciones (Portal Nacional de Datos Abiertos)

* **Descripción:** Catálogo oficial de estaciones, portales y zonas de transporte masivo.
* **Formato:** CSV / JSON.
* **Fecha de descarga:** 20/10/2026.
* **Licencia:** Creative Commons Attribution 4.0 (CC BY 4.0).
* **Procedencia y pasos:**
  - **URL oficial:** [Portal Nacional de Datos Abiertos de Colombia](https://www.datos.gov.co/browse?q=transporte%20masivo%20bogota)
  - **Pasos para obtenerla:** Ingresar al enlace del portal, filtrar por conjuntos de datos de transporte masivo en Bogotá, y descargar el archivo de estaciones/zonas en formato CSV.

## 3. Fuente F3: Trazados y Paraderos Troncales

* **Descripción:** Información geoespacial, de rutas, trazados y paraderos del sistema.
* **Formato:** JSON / CSV.
* **Fecha de descarga:** 20/10/2026.
* **Licencia:** Open Database License (ODbL).
* **Procedencia y pasos:**
  - **URL oficial:** [Portal de Datos Abiertos de la Secretaría de Movilidad](https://datos.movilidadbogota.gov.co/) o el [sitio de Datos Abiertos TransMilenio S.A.](https://datosabiertos-transmilenio.hub.arcgis.com/)
  - **Pasos para obtenerla:** Navegar al portal de movilidad de Bogotá, buscar los trazados de rutas troncales e interconectoras, y exportar los datos correspondientes al periodo 2024-2025.
