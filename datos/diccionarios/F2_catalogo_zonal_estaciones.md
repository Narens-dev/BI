# Diccionario de datos — Fuente F2: Portal Datos Abiertos (Catálogo Zonal y Estaciones)

Archivo: [`/datos/raw/Estaciones_Troncales_de_TRANSMILENIO.csv`](../raw/Estaciones_Troncales_de_TRANSMILENIO.csv)

| Campo | Tipo | Descripción | Ejemplo | Problema de calidad |
|---|---|---|---|---|
| codigo_estacion | VARCHAR | Identificador único oficial de la estación o paradero. | EST_045 | Ninguno |
| nombre_estacion | VARCHAR | Nombre público de la estación o portal. | Portal Norte | Inconsistencias menores en caracteres especiales/acentos. |
| zona | VARCHAR | Zona geográfica de planificación dentro de Bogotá. | Suba | Ninguno |
| corredor_vial | VARCHAR | Troncal o avenida principal asociada. | AutoNorte | Nulos en paraderos zonales de calles secundarias. |
