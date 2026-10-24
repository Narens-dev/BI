# Diccionario de datos — Fuente F1: Registro transaccional de validaciones

Archivo: [`/datos/raw/Dataset_registros.csv`](../raw/Dataset_registros.csv)

| Campo | Tipo | Descripción | Ejemplo | Problema de calidad |
|---|---|---|---|---|
| id_validacion | INTEGER | Identificador único de la transacción de validación. | 100245 | Ninguno (clave primaria limpia) |
| fecha_hora | VARCHAR / TIMESTAMP | Fecha y hora en que el usuario valida el pasaje. | 2024-10-15 07:32:10 | S1: Formato inconsistente de fechas (DD/MM/YYYY vs YYYY-MM-DD). |
| id_estacion | INTEGER | Código de la estación o paradero donde ocurrió la validación. | EST_045 | S2: Presencia de valores nulos/vacíos en transacciones de buses zonales. |
| id_ruta | VARCHAR | Código identificador de la ruta del bus. | F14 | Ninguno |
| id_tarjeta | VARCHAR | Código encriptado del medio de pago utilizado. | TJ_998341 | Ninguno |
| monto_tarifa | NUMERIC | Valor cobrado por la validación. | 2.950 | S4: Registros aislados con montos negativos o valores atípicos de cero. |
