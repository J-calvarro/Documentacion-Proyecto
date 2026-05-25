# Anexo — Catálogo completo de medidas DAX (111)

Modelo: `Estructura_AGRU_PRUEBA_v3`
Fuente: exportación `INFO.VIEW.MEASURES()` del modelo semántico.
Total medidas: **111**

---

## Índice rápido

| # | Tabla | Medida | Carpeta |
|---|-------|--------|---------|
| 1 | Fact_AccumSnapshot_Pedidos | # Cobrados | Volumen |
| 2 | Fact_AccumSnapshot_Pedidos | # Entregados | Volumen |
| 3 | Fact_AccumSnapshot_Pedidos | # Entregas a Tiempo | Eficacia Pipeline |
| 4 | Fact_AccumSnapshot_Pedidos | # Facturados | Volumen |
| 5 | Fact_AccumSnapshot_Pedidos | # Pedidos | Volumen |
| 6 | Fact_AccumSnapshot_Pedidos | # Pedidos Activos | Volumen |
| 7 | Fact_AccumSnapshot_Pedidos | # Pedidos En Curso | Pipeline |
| 8 | Fact_AccumSnapshot_Pedidos | % Conversion Factura-Cobro | Importes |
| 9 | Fact_AccumSnapshot_Pedidos | % OTIF (On Time In Full) | Eficacia Pipeline |
| 10 | Fact_AccumSnapshot_Pedidos | % Tasa Cobro | Eficacia Pipeline |
| 11 | Fact_AccumSnapshot_Pedidos | % Tasa Entrega | Eficacia Pipeline |
| 12 | Fact_AccumSnapshot_Pedidos | % Tasa Facturacion | Eficacia Pipeline |
| 13 | Fact_AccumSnapshot_Pedidos | Avg Ciclo Total | Tiempos de Ciclo |
| 14 | Fact_AccumSnapshot_Pedidos | Avg Dias Entrega a Factura | Tiempos de Ciclo |
| 15 | Fact_AccumSnapshot_Pedidos | Avg Dias Factura a Cobro | Tiempos de Ciclo |
| 16 | Fact_AccumSnapshot_Pedidos | Avg Dias Pedido a Entrega | Tiempos de Ciclo |
| 17 | Fact_AccumSnapshot_Pedidos | Avg Retraso Entrega | Tiempos de Ciclo |
| 18 | Fact_AccumSnapshot_Pedidos | Etiqueta Estado Facturacion Pedido | Trazabilidad pedido |
| 19 | Fact_AccumSnapshot_Pedidos | Importe Cobrado Acumulado YTD | Acumulados |
| 20 | Fact_AccumSnapshot_Pedidos | Importe Pedido Acumulado YTD | Acumulados |
| 21 | Fact_AccumSnapshot_Pedidos | Importe Pedidos por Etapa | Pipeline |
| 22 | Fact_AccumSnapshot_Pedidos | Importe Pendiente Cobrar | Importes |
| 23 | Fact_AccumSnapshot_Pedidos | Importe Pendiente Facturacion Pedido | Visuales comerciales |
| 24 | Fact_AccumSnapshot_Pedidos | Importe Total Cobrado | Importes |
| 25 | Fact_AccumSnapshot_Pedidos | Importe Total Facturado | Importes |
| 26 | Fact_AccumSnapshot_Pedidos | Importe Total Pedido | Importes |
| 27 | Fact_AccumSnapshot_Pedidos | Importe por Fecha Cobro | Role-Playing Fechas |
| 28 | Fact_AccumSnapshot_Pedidos | Importe por Fecha Entrega | Role-Playing Fechas |
| 29 | Fact_AccumSnapshot_Pedidos | Importe por Fecha Factura | Role-Playing Fechas |
| 30 | Fact_AccumSnapshot_Pedidos | Importe x Etapa Cobrado | Pipeline |
| 31 | Fact_AccumSnapshot_Pedidos | Importe x Etapa Entregado | Pipeline |
| 32 | Fact_AccumSnapshot_Pedidos | Importe x Etapa Facturado | Pipeline |
| 33 | Fact_AccumSnapshot_Pedidos | Importe x Etapa Pedido | Pipeline |
| 34 | Fact_AccumSnapshot_Pedidos | Max Dias Ciclo Acumulado | Tiempos de Ciclo |
| 35 | Fact_AccumSnapshot_Pedidos | Pedidos Cobrados por Fecha Cobro | Role-Playing Fechas |
| 36 | Fact_AccumSnapshot_Pedidos | Pedidos Entregados por Fecha Entrega | Role-Playing Fechas |
| 37 | Fact_AccumSnapshot_Pedidos | Snapshot Pedidos Acumulado | Acumulados |
| 38 | Fact_AcuerdosGlobales_Lineas | % Completado cantidad contrato | Visuales comerciales |
| 39 | Fact_AcuerdosGlobales_Lineas | Cantidad Pendiente Servir Contrato | Trazabilidad contrato |
| 40 | Fact_AcuerdosGlobales_Lineas | Cantidad Plan Acuerdos | Visuales comerciales |
| 41 | Fact_AcuerdosGlobales_Lineas | Cantidad Servida Contrato | Contrato vs pedidos |
| 42 | Fact_AcuerdosGlobales_Lineas | Importe Facturado Contrato | Trazabilidad contrato |
| 43 | Fact_AcuerdosGlobales_Lineas | Importe Pendiente Facturar Contrato | Trazabilidad contrato |
| 44 | Fact_AcuerdosGlobales_Lineas | Importe Plan Acuerdos | Visuales comerciales |
| 45 | Fact_AcuerdosGlobales_Lineas | Lista Fechas Entrega Contrato | Trazabilidad contrato |
| 46 | Fact_AcuerdosGlobales_Lineas | Primera Fecha Entrega Contrato | Trazabilidad contrato |
| 47 | Fact_AcuerdosGlobales_Lineas | Ultima Fecha Entrega Contrato | Trazabilidad contrato |
| 48 | Fact_AcuerdosGlobales_Lineas | importe_linea_cantidad_servida | Contrato vs pedidos |
| 49 | Fact_AcuerdosGlobales_Lineas | importe_linea_cantxprec | — |
| 50 | Fact_Albaranes_Lineas | # Albaranes Distintos | Volumen |
| 51 | Fact_Albaranes_Lineas | # Lineas Albaran | Volumen |
| 52 | Fact_Albaranes_Lineas | % Margen Bruto Entregas | Rentabilidad |
| 53 | Fact_Albaranes_Lineas | Cantidad Entregada | Cantidades |
| 54 | Fact_Albaranes_Lineas | DocNum Pedido Origen | Trazabilidad logística |
| 55 | Fact_Albaranes_Lineas | Importe Con IVA Entregas | IVA |
| 56 | Fact_Albaranes_Lineas | Importe Coste Entregas | Rentabilidad |
| 57 | Fact_Albaranes_Lineas | Importe Descuento Entregas | Descuentos |
| 58 | Fact_Albaranes_Lineas | Importe Entregado Lineas | Importes |
| 59 | Fact_Albaranes_Lineas | Importe IVA Entregas | IVA |
| 60 | Fact_Albaranes_Lineas | Kg Brutos Linea Albaran | Trazabilidad logística |
| 61 | Fact_Albaranes_Lineas | Margen Bruto Entregas | Rentabilidad |
| 62 | Fact_Facturas_Lineas | # Facturas Distintas | Volumen |
| 63 | Fact_Facturas_Lineas | # Lineas Factura | Volumen |
| 64 | Fact_Facturas_Lineas | % Descuento Medio Facturas | Descuentos |
| 65 | Fact_Facturas_Lineas | % Margen Bruto Facturas | Rentabilidad |
| 66 | Fact_Facturas_Lineas | Cantidad Facturada | Cantidades |
| 67 | Fact_Facturas_Lineas | Cantidad Neta Facturada | Cantidades |
| 68 | Fact_Facturas_Lineas | Importe Con IVA Facturas | IVA |
| 69 | Fact_Facturas_Lineas | Importe Coste Facturas | Rentabilidad |
| 70 | Fact_Facturas_Lineas | Importe Descuento Facturas | Descuentos |
| 71 | Fact_Facturas_Lineas | Importe Facturado Lineas | Importes |
| 72 | Fact_Facturas_Lineas | Importe IVA Facturas | IVA |
| 73 | Fact_Facturas_Lineas | Margen Bruto Facturas | Rentabilidad |
| 74 | Fact_Facturas_Lineas | Precio Medio Venta | Importes |
| 75 | Fact_Inventario_Almacen | articulos_cant_neta_insuficiente | — |
| 76 | Fact_Inventario_Almacen | articulos_no_disponibles | — |
| 77 | Fact_Ofertas_Lineas | Num Pedidos Generados desde Oferta | Trazabilidad oferta |
| 78 | Fact_Pedidos_Lineas | # Lineas Pedido | Volumen |
| 79 | Fact_Pedidos_Lineas | # Pedidos Distintos | Volumen |
| 80 | Fact_Pedidos_Lineas | % Completado cantidad pedido (paralelo contrato) | Paralelo contratos (pedido) |
| 81 | Fact_Pedidos_Lineas | % Completado importe pedido (paralelo contrato) | Paralelo contratos (pedido) |
| 82 | Fact_Pedidos_Lineas | % Cumplimiento Lineas | Ratios |
| 83 | Fact_Pedidos_Lineas | % Descuento Medio Pedidos | Descuentos |
| 84 | Fact_Pedidos_Lineas | % Margen Bruto Pedidos | Rentabilidad |
| 85 | Fact_Pedidos_Lineas | Cantidad Devuelta Linea Pedido | Trazabilidad pedido |
| 86 | Fact_Pedidos_Lineas | Cantidad Facturada Linea Pedido | Trazabilidad |
| 87 | Fact_Pedidos_Lineas | Cantidad Pedida | Cantidades |
| 88 | Fact_Pedidos_Lineas | Cantidad Pendiente | Cantidades |
| 89 | Fact_Pedidos_Lineas | Cantidad Pendiente Servir Pedido Linea | Paralelo contratos (pedido) |
| 90 | Fact_Pedidos_Lineas | Cantidad Servida Cumplida Pedido Linea | Paralelo contratos (pedido) |
| 91 | Fact_Pedidos_Lineas | Cantidad Servida Linea Pedido | Trazabilidad |
| 92 | Fact_Pedidos_Lineas | Cantidad Solicitud Devolucion Linea Pedido | Trazabilidad pedido |
| 93 | Fact_Pedidos_Lineas | Dias Pedido a Primera Entrega Linea | Trazabilidad pedido |
| 94 | Fact_Pedidos_Lineas | Etiqueta Cobertura Stock Linea | Trazabilidad pedido |
| 95 | Fact_Pedidos_Lineas | Filtrar por Cobertura | — |
| 96 | Fact_Pedidos_Lineas | Importe Abonos Linea Pedido | Trazabilidad pedido |
| 97 | Fact_Pedidos_Lineas | Importe Con IVA Pedidos | IVA |
| 98 | Fact_Pedidos_Lineas | Importe Coste Pedidos | Rentabilidad |
| 99 | Fact_Pedidos_Lineas | Importe Descuento Pedidos | Descuentos |
| 100 | Fact_Pedidos_Lineas | Importe IVA Pedidos | IVA |
| 101 | Fact_Pedidos_Lineas | Importe Pedido Lineas | Importes |
| 102 | Fact_Pedidos_Lineas | Importe Pendiente Facturar Plan vs Fact Pedido | Paralelo contratos (pedido) |
| 103 | Fact_Pedidos_Lineas | Importe facturación Linea | Trazabilidad pedido |
| 104 | Fact_Pedidos_Lineas | Importe pendiente Facturado Linea Pedido | Trazabilidad pedido |
| 105 | Fact_Pedidos_Lineas | Lineas Pendientes Sin Stock Suficiente | Trazabilidad |
| 106 | Fact_Pedidos_Lineas | Lista Fechas Entrega Pedido Linea | Paralelo contratos (pedido) |
| 107 | Fact_Pedidos_Lineas | Margen Bruto Pedidos | Rentabilidad |
| 108 | Fact_Pedidos_Lineas | Primera Fecha Entrega Pedido Linea | Paralelo contratos (pedido) |
| 109 | Fact_Pedidos_Lineas | Stock Neto Servible Linea Actual | Trazabilidad pedido |
| 110 | Fact_Pedidos_Lineas | Stock Neto Servible Linea Pedido | Trazabilidad |
| 111 | Fact_Pedidos_Lineas | Ultima Fecha Entrega Pedido Linea | Paralelo contratos (pedido) |

---

## Expresiones DAX por tabla

### Fact_AccumSnapshot_Pedidos (37 medidas)

#### 1. [# Cobrados]
- **Carpeta:** Volumen
- **Descripción:** Pedidos que han llegado al hito de cobro

```dax
SUMX(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Cobrado])
```

#### 2. [# Entregados]
- **Carpeta:** Volumen
- **Descripción:** Pedidos que han llegado al hito de entrega

```dax
SUMX(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Entregado])
```

#### 3. [# Entregas a Tiempo]
- **Carpeta:** Eficacia Pipeline
- **Descripción:** Pedidos entregados a tiempo o antes (retraso <= 0)

```dax
COUNTROWS(FILTER(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Entregado] = 1 && Fact_AccumSnapshot_Pedidos[Dias_Retraso_Entrega] <= 0))
```

#### 4. [# Facturados]
- **Carpeta:** Volumen
- **Descripción:** Pedidos que han llegado al hito de factura

```dax
SUMX(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Facturado])
```

#### 5. [# Pedidos]
- **Carpeta:** Volumen
- **Descripción:** Número total de pedidos

```dax
COUNTROWS(Fact_AccumSnapshot_Pedidos)
```

#### 6. [# Pedidos Activos]
- **Carpeta:** Volumen
- **Descripción:** Pedidos no cancelados

```dax
COUNTROWS(FILTER(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Cancelado] <> "Y"))
```

#### 7. [# Pedidos En Curso]
- **Carpeta:** Pipeline
- **Descripción:** Pedidos activos que aún no han sido cobrados

```dax
COUNTROWS(FILTER(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Cancelado] <> "Y" && Fact_AccumSnapshot_Pedidos[Flag_Cobrado] = 0))
```

#### 8. [% Conversion Factura-Cobro]
- **Carpeta:** Importes
- **Descripción:** Porcentaje del importe facturado que ya ha sido cobrado

```dax
DIVIDE([Importe Total Cobrado], [Importe Total Facturado], 0)
```

#### 9. [% OTIF (On Time In Full)]
- **Carpeta:** Eficacia Pipeline
- **Descripción:** Porcentaje de entregas realizadas a tiempo sobre el total de pedidos activos entregados

```dax
DIVIDE([# Entregas a Tiempo], [# Entregados], 0)
```

#### 10. [% Tasa Cobro]
- **Carpeta:** Eficacia Pipeline
- **Descripción:** Porcentaje de pedidos activos cobrados

```dax
DIVIDE([# Cobrados], [# Pedidos Activos], 0)
```

#### 11. [% Tasa Entrega]
- **Carpeta:** Eficacia Pipeline
- **Descripción:** Porcentaje de pedidos activos entregados

```dax
DIVIDE([# Entregados], [# Pedidos Activos], 0)
```

#### 12. [% Tasa Facturacion]
- **Carpeta:** Eficacia Pipeline
- **Descripción:** Porcentaje de pedidos activos facturados

```dax
DIVIDE([# Facturados], [# Pedidos Activos], 0)
```

#### 13. [Avg Ciclo Total]
- **Carpeta:** Tiempos de Ciclo
- **Descripción:** Duración media del ciclo completo (pedido a cobro) para pedidos completados

```dax
AVERAGEX(FILTER(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Cobrado] = 1), Fact_AccumSnapshot_Pedidos[Dias_Ciclo_Acumulado])
```

#### 14. [Avg Dias Entrega a Factura]
- **Carpeta:** Tiempos de Ciclo
- **Descripción:** Tiempo medio (días) desde entrega hasta facturación

```dax
AVERAGEX(FILTER(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Facturado] = 1 && NOT(ISBLANK(Fact_AccumSnapshot_Pedidos[Dias_Entrega_a_Factura]))), Fact_AccumSnapshot_Pedidos[Dias_Entrega_a_Factura])
```

#### 15. [Avg Dias Factura a Cobro]
- **Carpeta:** Tiempos de Ciclo
- **Descripción:** Tiempo medio (días) desde factura hasta cobro (DSO - Days Sales Outstanding)

```dax
AVERAGEX(FILTER(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Cobrado] = 1 && NOT(ISBLANK(Fact_AccumSnapshot_Pedidos[Dias_Factura_a_Cobro]))), Fact_AccumSnapshot_Pedidos[Dias_Factura_a_Cobro])
```

#### 16. [Avg Dias Pedido a Entrega]
- **Carpeta:** Tiempos de Ciclo
- **Descripción:** Tiempo medio (días) desde pedido hasta primera entrega - sólo pedidos entregados

```dax
AVERAGEX(FILTER(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Entregado] = 1 && NOT(ISBLANK(Fact_AccumSnapshot_Pedidos[Dias_Pedido_a_Entrega]))), Fact_AccumSnapshot_Pedidos[Dias_Pedido_a_Entrega])
```

#### 17. [Avg Retraso Entrega]
- **Carpeta:** Tiempos de Ciclo
- **Descripción:** Retraso medio en entrega vs fecha solicitada (positivo=tarde, negativo=adelantado)

```dax
AVERAGEX(FILTER(Fact_AccumSnapshot_Pedidos, Fact_AccumSnapshot_Pedidos[Flag_Entregado] = 1 && NOT(ISBLANK(Fact_AccumSnapshot_Pedidos[Dias_Retraso_Entrega]))), Fact_AccumSnapshot_Pedidos[Dias_Retraso_Entrega])
```

#### 18. [Etiqueta Estado Facturacion Pedido]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Estado textual del pedido según importe pedido vs facturado en snapshot de cabecera.

```dax
VAR impF = MAX ( 'Fact_AccumSnapshot_Pedidos'[Importe_Facturado] )
VAR impP = MAX ( 'Fact_AccumSnapshot_Pedidos'[Importe_Pedido] )
RETURN
    SWITCH (
        TRUE (),
        ISBLANK ( impP ) || impP = 0, BLANK (),
        ISBLANK ( impF ) || impF <= 0, "Sin facturar",
        impF >= impP - 0.01, "Facturado",
        "Facturación parcial"
    )
```

#### 19. [Importe Cobrado Acumulado YTD]
- **Carpeta:** Acumulados
- **Descripción:** Importe cobrado acumulado en el año hasta la fecha (filtrado por fecha de cobro)

```dax
CALCULATE([Importe Total Cobrado], USERELATIONSHIP(Fact_AccumSnapshot_Pedidos[Fecha_Cobro], Dim_Fecha[Date]), DATESYTD(Dim_Fecha[Date]))
```

#### 20. [Importe Pedido Acumulado YTD]
- **Carpeta:** Acumulados
- **Descripción:** Importe total de pedidos acumulado en el año hasta la fecha

```dax
CALCULATE([Importe Total Pedido], DATESYTD(Dim_Fecha[Date]))
```

#### 21. [Importe Pedidos por Etapa]
- **Carpeta:** Pipeline
- **Descripción:** Importe total de pedidos segmentado por etapa del pipeline

```dax
CALCULATE([Importe Total Pedido])
```

#### 22. [Importe Pendiente Cobrar]
- **Carpeta:** Importes
- **Descripción:** Importe facturado pendiente de cobro

```dax
[Importe Total Facturado] - [Importe Total Cobrado]
```

#### 23. [Importe Pendiente Facturacion Pedido]
- **Carpeta:** Visuales comerciales
- **Descripción:** Importe total de pedido menos facturado a nivel cabecera (snapshot). Validar escenarios de facturación parcial o prepago.

```dax
[Importe Total Pedido] - [Importe Total Facturado]
```

#### 24. [Importe Total Cobrado]
- **Carpeta:** Importes
- **Descripción:** Suma del importe cobrado

```dax
SUM(Fact_AccumSnapshot_Pedidos[Importe_Cobrado])
```

#### 25. [Importe Total Facturado]
- **Carpeta:** Importes
- **Descripción:** Suma del importe facturado

```dax
SUM(Fact_AccumSnapshot_Pedidos[Importe_Facturado])
```

#### 26. [Importe Total Pedido]
- **Carpeta:** Importes
- **Descripción:** Suma del importe total de pedidos

```dax
SUM(Fact_AccumSnapshot_Pedidos[Importe_Pedido])
```

#### 27. [Importe por Fecha Cobro]
- **Carpeta:** Role-Playing Fechas
- **Descripción:** [Role-playing] Importe cobrado filtrado por fecha de COBRO (usa relación inactiva)

```dax
CALCULATE([Importe Total Cobrado], USERELATIONSHIP(Fact_AccumSnapshot_Pedidos[Fecha_Cobro], Dim_Fecha[Date]))
```

#### 28. [Importe por Fecha Entrega]
- **Carpeta:** Role-Playing Fechas
- **Descripción:** [Role-playing] Importe de pedidos filtrado por fecha de ENTREGA (usa relación inactiva). Kimball: USERELATIONSHIP para cambiar el hito de fecha.

```dax
CALCULATE([Importe Total Pedido], USERELATIONSHIP(Fact_AccumSnapshot_Pedidos[Fecha_Entrega], Dim_Fecha[Date]))
```

#### 29. [Importe por Fecha Factura]
- **Carpeta:** Role-Playing Fechas
- **Descripción:** [Role-playing] Importe de pedidos filtrado por fecha de FACTURA (usa relación inactiva)

```dax
CALCULATE([Importe Total Facturado], USERELATIONSHIP(Fact_AccumSnapshot_Pedidos[Fecha_Factura], Dim_Fecha[Date]))
```

#### 30. [Importe x Etapa Cobrado]
- **Carpeta:** Pipeline
- **Descripción:** Pedidos completados en hito Cobrado

```dax
CALCULATE([Importe Total Pedido], Fact_AccumSnapshot_Pedidos[Etapa_Actual] = "4-Cobrado")
```

#### 31. [Importe x Etapa Entregado]
- **Carpeta:** Pipeline
- **Descripción:** Pedidos en hito Entregado (entregados pero sin factura)

```dax
CALCULATE([Importe Total Pedido], Fact_AccumSnapshot_Pedidos[Etapa_Actual] = "2-Entregado")
```

#### 32. [Importe x Etapa Facturado]
- **Carpeta:** Pipeline
- **Descripción:** Pedidos en hito Facturado (facturados pero sin cobro)

```dax
CALCULATE([Importe Total Pedido], Fact_AccumSnapshot_Pedidos[Etapa_Actual] = "3-Facturado")
```

#### 33. [Importe x Etapa Pedido]
- **Carpeta:** Pipeline
- **Descripción:** Pedidos en hito Pedido (sin entrega aún)

```dax
CALCULATE([Importe Total Pedido], Fact_AccumSnapshot_Pedidos[Etapa_Actual] = "1-Pedido")
```

#### 34. [Max Dias Ciclo Acumulado]
- **Carpeta:** Tiempos de Ciclo
- **Descripción:** Máximo de días de ciclo (para identificar outliers)

```dax
MAXX(FILTER(Fact_AccumSnapshot_Pedidos, NOT(ISBLANK(Fact_AccumSnapshot_Pedidos[Dias_Ciclo_Acumulado]))), Fact_AccumSnapshot_Pedidos[Dias_Ciclo_Acumulado])
```

#### 35. [Pedidos Cobrados por Fecha Cobro]
- **Carpeta:** Role-Playing Fechas
- **Descripción:** [Role-playing] Pedidos cobrados filtrado por fecha de cobro

```dax
CALCULATE([# Cobrados], USERELATIONSHIP(Fact_AccumSnapshot_Pedidos[Fecha_Cobro], Dim_Fecha[Date]))
```

#### 36. [Pedidos Entregados por Fecha Entrega]
- **Carpeta:** Role-Playing Fechas
- **Descripción:** [Role-playing] Pedidos entregados filtrado por fecha de entrega

```dax
CALCULATE([# Entregados], USERELATIONSHIP(Fact_AccumSnapshot_Pedidos[Fecha_Entrega], Dim_Fecha[Date]))
```

#### 37. [Snapshot Pedidos Acumulado]
- **Carpeta:** Acumulados
- **Descripción:** Acumula el recuento de pedidos hasta la fecha (YTD). Demuestra la naturaleza acumulativa del patrón.

```dax
CALCULATE([# Pedidos], DATESYTD(Dim_Fecha[Date]))
```

### Fact_Pedidos_Lineas (34 medidas)

#### 38. [# Lineas Pedido]
- **Carpeta:** Volumen
- **Descripción:** Número de líneas de pedido

```dax
COUNTROWS(Fact_Pedidos_Lineas)
```

#### 39. [# Pedidos Distintos]
- **Carpeta:** Volumen

```dax
DISTINCTCOUNT(Fact_Pedidos_Lineas[DocNum])
```

#### 40. [% Completado cantidad pedido (paralelo contrato)]
- **Carpeta:** Paralelo contratos (pedido)
- **Descripción:** Paralelo a % Completado cantidad contrato: cumplida SAP / cantidad pedida.

```dax
DIVIDE (
    SUM ( Fact_Pedidos_Lineas[Cantidad_Cumplida] ),
    SUM ( Fact_Pedidos_Lineas[Cantidad] )
)
```

#### 41. [% Completado importe pedido (paralelo contrato)]
- **Carpeta:** Paralelo contratos (pedido)

```dax
1 -  DIVIDE (
   [Importe x Etapa Entregado], [Importe x Etapa Facturado]
)
```

#### 42. [% Cumplimiento Lineas]
- **Carpeta:** Ratios

```dax
DIVIDE(SUM(Fact_Pedidos_Lineas[Cantidad]) - SUM(Fact_Pedidos_Lineas[Cantidad_Pendiente]), SUM(Fact_Pedidos_Lineas[Cantidad]), 0)
```

#### 43. [% Descuento Medio Pedidos]
- **Carpeta:** Descuentos

```dax
DIVIDE(SUM(Fact_Pedidos_Lineas[Importe_Descuento]), SUM(Fact_Pedidos_Lineas[Precio_Tarifa]) * SUM(Fact_Pedidos_Lineas[Cantidad]), 0)
```

#### 44. [% Margen Bruto Pedidos]
- **Carpeta:** Rentabilidad

```dax
DIVIDE(SUM(Fact_Pedidos_Lineas[Margen_Bruto]), SUM(Fact_Pedidos_Lineas[Importe_Linea]), 0)
```

#### 45. [Cantidad Devuelta Linea Pedido]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Devoluciones cuyo origen apunta a la línea de pedido (ObjectType 17=ORDR). Ajustar si en origen usáis factura o entrega.

```dax
SUMX (
    'Fact_Pedidos_Lineas',
    VAR de = 'Fact_Pedidos_Lineas'[DocEntry]
    VAR ln = 'Fact_Pedidos_Lineas'[LineNum]
    RETURN
        CALCULATE (
            SUM ( 'Fact_Devoluciones_Lineas'[Cantidad] ),
            FILTER (
                ALL ( 'Fact_Devoluciones_Lineas' ),
                'Fact_Devoluciones_Lineas'[DocOrigen_ObjectType] = 17
                    && 'Fact_Devoluciones_Lineas'[DocOrigen_Entry] = de
                    && 'Fact_Devoluciones_Lineas'[DocOrigen_Line] = ln
            )
        )
)
```

#### 46. [Cantidad Facturada Linea Pedido]
- **Carpeta:** Trazabilidad
- **Descripción:** Facturas enlazadas por Pedido_Line_Key directo o por líneas de albarán del pedido. Si un documento aparece en ambos caminos, revisar datos de origen.

```dax
SUMX ( Fact_Pedidos_Lineas, VAR k = Fact_Pedidos_Lineas[Pedido_Line_Key] VAR direct = CALCULATE ( SUM ( Fact_Facturas_Lineas[Cantidad] ), FILTER ( ALL ( Fact_Facturas_Lineas ), Fact_Facturas_Lineas[Pedido_Line_Key] = k ) ) VAR viaDel = SUMX ( FILTER ( ALL ( Fact_Albaranes_Lineas ), Fact_Albaranes_Lineas[Pedido_Line_Key] = k ), VAR ak = Fact_Albaranes_Lineas[Albaran_Line_Key] RETURN CALCULATE ( SUM ( Fact_Facturas_Lineas[Cantidad] ), FILTER ( ALL ( Fact_Facturas_Lineas ), Fact_Facturas_Lineas[Albaran_Line_Key] = ak ) ) ) RETURN direct + viaDel )
```

#### 47. [Cantidad Pedida]
- **Carpeta:** Cantidades

```dax
SUM(Fact_Pedidos_Lineas[Cantidad])
```

#### 48. [Cantidad Pendiente]
- **Carpeta:** Cantidades

```dax
SUM(Fact_Pedidos_Lineas[Cantidad_Pendiente])
```

#### 49. [Cantidad Pendiente Servir Pedido Linea]
- **Carpeta:** Paralelo contratos (pedido)
- **Descripción:** Paralelo a Cantidad Pendiente Servir Contrato: cantidad pedida menos cumplida (misma fórmula que [Cantidad Plan] - [Cantidad Servida] en acuerdo).

```dax
SUM ( Fact_Pedidos_Lineas[Cantidad] ) - SUM ( Fact_Pedidos_Lineas[Cantidad_Cumplida] )
```

#### 50. [Cantidad Servida Cumplida Pedido Linea]
- **Carpeta:** Paralelo contratos (pedido)
- **Descripción:** Misma base que Cantidad Servida Contrato: suma de Cantidad_Cumplida en línea de pedido, sin TREATAS (el contexto es ya línea).

```dax
SUM ( Fact_Pedidos_Lineas[Cantidad_Cumplida] )
```

#### 51. [Cantidad Servida Linea Pedido]
- **Carpeta:** Trazabilidad
- **Descripción:** Cantidad entregada (albarán) enlazada a cada línea de pedido mediante Pedido_Line_Key.

```dax
SUMX ( Fact_Pedidos_Lineas, VAR k = Fact_Pedidos_Lineas[Pedido_Line_Key] RETURN CALCULATE ( SUM ( Fact_Albaranes_Lineas[Cantidad] ), FILTER ( ALL ( Fact_Albaranes_Lineas ), Fact_Albaranes_Lineas[Pedido_Line_Key] = k ) ) )
```

#### 52. [Cantidad Solicitud Devolucion Linea Pedido]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Solicitudes de devolución enlazadas a línea de pedido (ObjectType 17). Verificar ObjectType real en SAP.

```dax
SUMX (
    'Fact_Pedidos_Lineas',
    VAR de = 'Fact_Pedidos_Lineas'[DocEntry]
    VAR ln = 'Fact_Pedidos_Lineas'[LineNum]
    RETURN
        CALCULATE (
            SUM ( 'Fact_Solicitudes_Devolucion_Lineas'[Cantidad] ),
            FILTER (
                ALL ( 'Fact_Solicitudes_Devolucion_Lineas' ),
                'Fact_Solicitudes_Devolucion_Lineas'[DocOrigen_ObjectType] = 17
                    && 'Fact_Solicitudes_Devolucion_Lineas'[DocOrigen_Entry] = de
                    && 'Fact_Solicitudes_Devolucion_Lineas'[DocOrigen_Line] = ln
            )
        )
)
```

#### 53. [Dias Pedido a Primera Entrega Linea]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Días desde fecha de pedido hasta primer albarán de la línea. Usar en matriz/detalle con grano línea de pedido (Pedido_Line_Key o DocEntry+LineNum).

```dax
VAR k = SELECTEDVALUE ( 'Fact_Pedidos_Lineas'[Pedido_Line_Key] )
VAR fp = SELECTEDVALUE ( 'Fact_Pedidos_Lineas'[Fecha_Pedido] )
VAR fe =
    MINX (
        FILTER (
            ALL ( 'Fact_Albaranes_Lineas' ),
            'Fact_Albaranes_Lineas'[Pedido_Line_Key] = k
        ),
        'Fact_Albaranes_Lineas'[Fecha_Albaran]
    )
RETURN
    IF (
        ISBLANK ( k ) || ISBLANK ( fp ) || ISBLANK ( fe ),
        BLANK (),
        DATEDIFF ( fp, fe, DAY )
    )
```

#### 54. [Etiqueta Cobertura Stock Linea]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Evalúa si el stock del almacén de la línea cubre la cantidad pendiente.

```dax
VAR pend = SUM ( 'Fact_Pedidos_Lineas'[Cantidad_Pendiente] )
VAR stk = [Stock Neto Servible Linea Actual]
RETURN
    SWITCH (
        TRUE (),
        ISBLANK ( stk ), BLANK (),
        pend <= 0, "Sin pendiente",
        stk >= pend, "Stock suficiente",
        "Stock insuficiente"
    )
```

#### 55. [Filtrar por Cobertura]

```dax
VAR EtiquetaSeleccionada = SELECTEDVALUE(Tabla_Filtro_Cobertura[Etiqueta])
VAR EtiquetaActual = [Etiqueta Cobertura Stock Linea]
RETURN
    SWITCH(
        TRUE(),
        ISBLANK(EtiquetaSeleccionada), 1,
        EtiquetaSeleccionada = EtiquetaActual, 1,
        0
    )
```

#### 56. [Importe Abonos Linea Pedido]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Abonos/notas de crédito aplicados a líneas de factura que a su vez enlazan con esta línea de pedido (ObjectType 13=OINV).

```dax
SUMX (
    'Fact_Pedidos_Lineas',
    VAR k = 'Fact_Pedidos_Lineas'[Pedido_Line_Key]
    RETURN
        SUMX (
            FILTER (
                ALL ( 'Fact_Facturas_Lineas' ),
                'Fact_Facturas_Lineas'[Pedido_Line_Key] = k
            ),
            VAR fe = 'Fact_Facturas_Lineas'[DocEntry]
            VAR fl = 'Fact_Facturas_Lineas'[LineNum]
            RETURN
                CALCULATE (
                    SUM ( 'Fact_Abonos_Lineas'[Importe_Linea] ),
                    FILTER (
                        ALL ( 'Fact_Abonos_Lineas' ),
                        'Fact_Abonos_Lineas'[DocOrigen_ObjectType] = 13
                            && 'Fact_Abonos_Lineas'[DocOrigen_Entry] = fe
                            && 'Fact_Abonos_Lineas'[DocOrigen_Line] = fl
                    )
                )
        )
)
```

#### 57. [Importe Con IVA Pedidos]
- **Carpeta:** IVA

```dax
SUM(Fact_Pedidos_Lineas[Importe_Linea_ConIVA])
```

#### 58. [Importe Coste Pedidos]
- **Carpeta:** Rentabilidad

```dax
SUM(Fact_Pedidos_Lineas[Importe_Coste])
```

#### 59. [Importe Descuento Pedidos]
- **Carpeta:** Descuentos

```dax
SUM(Fact_Pedidos_Lineas[Importe_Descuento])
```

#### 60. [Importe IVA Pedidos]
- **Carpeta:** IVA

```dax
SUM(Fact_Pedidos_Lineas[Importe_IVA])
```

#### 61. [Importe Pedido Lineas]
- **Carpeta:** Importes

```dax
SUM(Fact_Pedidos_Lineas[Importe_Linea])
```

#### 62. [Importe Pendiente Facturar Plan vs Fact Pedido]
- **Carpeta:** Paralelo contratos (pedido)
- **Descripción:** Paralelo a Importe Pendiente Facturar Contrato: importe líneas de pedido menos importe facturado rastreado (diferente granularidad a Importe Pendiente Facturar Linea en modo SUMX por línea).

```dax
[Importe Pedido Lineas] - [Importe pendiente Facturado Linea Pedido]
```

#### 63. [Importe facturación Linea]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Importe de la línea de pedido pendiente de facturar (línea bruta SAP vs facturado rastreado).

```dax
SUMX (
    'Fact_Pedidos_Lineas',
    VAR k = 'Fact_Pedidos_Lineas'[Pedido_Line_Key]
    VAR impLinea = 'Fact_Pedidos_Lineas'[Importe_Linea]
    VAR impFac =
        CALCULATE (
            SUM ( 'Fact_Facturas_Lineas'[Importe_Linea] ),
            FILTER ( ALL ( 'Fact_Facturas_Lineas' ), 'Fact_Facturas_Lineas'[Pedido_Line_Key] = k )
        )
    RETURN
        impLinea - impFac
)
```

#### 64. [Importe pendiente Facturado Linea Pedido]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Importe facturado trazado a la línea de pedido (directo + vía albarán implícito en Pedido_Line_Key de factura). Coherente con Cantidad Facturada Linea Pedido.

```dax
var imp =SUMX (
    'Fact_Pedidos_Lineas',
    VAR k = 'Fact_Pedidos_Lineas'[Pedido_Line_Key]
    RETURN
        CALCULATE (
            SUM ( 'Fact_Facturas_Lineas'[Importe_Linea] ),
            FILTER ( ALL ( 'Fact_Facturas_Lineas' ), 'Fact_Facturas_Lineas'[Pedido_Line_Key] = k )
        )
)
return if (imp =BLANK(),0,imp)
```

#### 65. [Lineas Pendientes Sin Stock Suficiente]
- **Carpeta:** Trazabilidad
- **Descripción:** Recuento de líneas con pendiente > 0 y stock del almacén inferior al pendiente.

```dax
SUMX ( Fact_Pedidos_Lineas, VAR pend = Fact_Pedidos_Lineas[Cantidad_Pendiente] VAR stk = CALCULATE ( MAX ( Fact_Inventario_Almacen[Stock_Neta_Servible] ), FILTER ( ALL ( Fact_Inventario_Almacen ), Fact_Inventario_Almacen[ItemCode] = Fact_Pedidos_Lineas[ItemCode] && Fact_Inventario_Almacen[Almacen] = Fact_Pedidos_Lineas[Almacen] ) ) RETURN IF ( pend > 0 && stk < pend, 1, 0 ) )
```

#### 66. [Lista Fechas Entrega Pedido Linea]
- **Carpeta:** Paralelo contratos (pedido)
- **Descripción:** Como Lista Fechas Entrega Contrato, para línea(s) de pedido en contexto.

```dax
VAR PKset =
    VALUES ( Fact_Pedidos_Lineas[Pedido_Line_Key] )
VAR DatesTbl =
    DISTINCT (
        SELECTCOLUMNS (
            FILTER (
                ALL ( Fact_Albaranes_Lineas ),
                Fact_Albaranes_Lineas[Pedido_Line_Key] IN PKset
            ),
            "d", Fact_Albaranes_Lineas[Fecha_Albaran]
        )
    )
RETURN
    CONCATENATEX ( DatesTbl, FORMAT ( [d], "Short Date" ), ", ", [d], ASC )
```

#### 67. [Margen Bruto Pedidos]
- **Carpeta:** Rentabilidad

```dax
SUM(Fact_Pedidos_Lineas[Margen_Bruto])
```

#### 68. [Primera Fecha Entrega Pedido Linea]
- **Carpeta:** Paralelo contratos (pedido)
- **Descripción:** Como Primera Fecha Entrega Contrato, pero con conjunto de Pedido_Line_Key del contexto de fila.

```dax
VAR PKset =
    VALUES ( Fact_Pedidos_Lineas[Pedido_Line_Key] )
RETURN
    MINX (
        FILTER (
            ALL ( Fact_Albaranes_Lineas ),
            Fact_Albaranes_Lineas[Pedido_Line_Key] IN PKset
        ),
        Fact_Albaranes_Lineas[Fecha_Albaran]
    )
```

#### 69. [Stock Neto Servible Linea Actual]
- **Carpeta:** Trazabilidad pedido
- **Descripción:** Stock neta servible para la combinación ítem-almacén de la línea (detalle/matríz). Complementa Stock Neto Servible Linea Pedido agregado.

```dax
VAR ic = SELECTEDVALUE ( 'Fact_Pedidos_Lineas'[ItemCode] )
VAR alm = SELECTEDVALUE ( 'Fact_Pedidos_Lineas'[Almacen] )
RETURN
    IF (
        ISBLANK ( ic ) || ISBLANK ( alm ),
        BLANK (),
        CALCULATE (
            MAX ( 'Fact_Inventario_Almacen'[Stock_Neta_Servible] ),
            FILTER (
                ALL ( 'Fact_Inventario_Almacen' ),
                'Fact_Inventario_Almacen'[ItemCode] = ic
                    && 'Fact_Inventario_Almacen'[Almacen] = alm
            )
        )
    )
```

#### 70. [Stock Neto Servible Linea Pedido]
- **Carpeta:** Trazabilidad
- **Descripción:** Stock neta servible en el mismo almacén que la línea de pedido (OITW+OITM).

```dax
SUMX ( Fact_Pedidos_Lineas, CALCULATE ( MAX ( Fact_Inventario_Almacen[Stock_Neta_Servible] ), FILTER ( ALL ( Fact_Inventario_Almacen ), Fact_Inventario_Almacen[ItemCode] = Fact_Pedidos_Lineas[ItemCode] && Fact_Inventario_Almacen[Almacen] = Fact_Pedidos_Lineas[Almacen] ) ) )
```

#### 71. [Ultima Fecha Entrega Pedido Linea]
- **Carpeta:** Paralelo contratos (pedido)
- **Descripción:** Como Ultima Fecha Entrega Contrato, a nivel línea de pedido.

```dax
VAR PKset =
    VALUES ( Fact_Pedidos_Lineas[Pedido_Line_Key] )
RETURN
    MAXX (
        FILTER (
            ALL ( Fact_Albaranes_Lineas ),
            Fact_Albaranes_Lineas[Pedido_Line_Key] IN PKset
        ),
        Fact_Albaranes_Lineas[Fecha_Albaran]
    )
```

### Fact_Albaranes_Lineas (12 medidas)

#### 72. [# Albaranes Distintos]
- **Carpeta:** Volumen

```dax
DISTINCTCOUNT(Fact_Albaranes_Lineas[DocNum])
```

#### 73. [# Lineas Albaran]
- **Carpeta:** Volumen

```dax
COUNTROWS(Fact_Albaranes_Lineas)
```

#### 74. [% Margen Bruto Entregas]
- **Carpeta:** Rentabilidad

```dax
DIVIDE(SUM(Fact_Albaranes_Lineas[Margen_Bruto]), SUM(Fact_Albaranes_Lineas[Importe_Linea]), 0)
```

#### 75. [Cantidad Entregada]
- **Carpeta:** Cantidades

```dax
SUM(Fact_Albaranes_Lineas[Cantidad])
```

#### 76. [DocNum Pedido Origen]
- **Carpeta:** Trazabilidad logística
- **Descripción:** Número de pedido visible para la línea de albarán (lookup por Pedido_DocEntry). Útil en tabla logística tipo captura.

```dax
IF (
    ISBLANK ( MAX ( 'Fact_Albaranes_Lineas'[Pedido_DocEntry] ) ),
    BLANK (),
    LOOKUPVALUE (
        'Fact_AccumSnapshot_Pedidos'[DocNum],
        'Fact_AccumSnapshot_Pedidos'[DocEntry], MAX ( 'Fact_Albaranes_Lineas'[Pedido_DocEntry] )
    )
)
```

#### 77. [Importe Con IVA Entregas]
- **Carpeta:** IVA

```dax
SUM(Fact_Albaranes_Lineas[Importe_Linea_ConIVA])
```

#### 78. [Importe Coste Entregas]
- **Carpeta:** Rentabilidad

```dax
SUM(Fact_Albaranes_Lineas[Importe_Coste])
```

#### 79. [Importe Descuento Entregas]
- **Carpeta:** Descuentos

```dax
SUM(Fact_Albaranes_Lineas[Importe_Descuento])
```

#### 80. [Importe Entregado Lineas]
- **Carpeta:** Importes

```dax
SUM(Fact_Albaranes_Lineas[Importe_Linea])
```

#### 81. [Importe IVA Entregas]
- **Carpeta:** IVA

```dax
SUM(Fact_Albaranes_Lineas[Importe_IVA])
```

#### 82. [Kg Brutos Linea Albaran]
- **Carpeta:** Trazabilidad logística
- **Descripción:** Suma de peso bruto por línea de albarán (equivalente a columnas del ejemplo).

```dax
SUM ( 'Fact_Albaranes_Lineas'[Peso_Line_Kg] )
```

#### 83. [Margen Bruto Entregas]
- **Carpeta:** Rentabilidad

```dax
SUM(Fact_Albaranes_Lineas[Margen_Bruto])
```

### Fact_Facturas_Lineas (13 medidas)

#### 84. [# Facturas Distintas]
- **Carpeta:** Volumen

```dax
DISTINCTCOUNT(Fact_Facturas_Lineas[DocNum])
```

#### 85. [# Lineas Factura]
- **Carpeta:** Volumen

```dax
COUNTROWS(Fact_Facturas_Lineas)
```

#### 86. [% Descuento Medio Facturas]
- **Carpeta:** Descuentos

```dax
DIVIDE(SUM(Fact_Facturas_Lineas[Importe_Descuento]), SUM(Fact_Facturas_Lineas[Importe_Descuento]) + SUM(Fact_Facturas_Lineas[Importe_Linea]), 0)
```

#### 87. [% Margen Bruto Facturas]
- **Carpeta:** Rentabilidad
- **Descripción:** KPI clave de rentabilidad real en ventas facturadas

```dax
DIVIDE(SUM(Fact_Facturas_Lineas[Margen_Bruto]), SUM(Fact_Facturas_Lineas[Importe_Linea]), 0)
```

#### 88. [Cantidad Facturada]
- **Carpeta:** Cantidades

```dax
SUM(Fact_Facturas_Lineas[Cantidad])
```

#### 89. [Cantidad Neta Facturada]
- **Carpeta:** Cantidades
- **Descripción:** Cantidad facturada menos devoluciones

```dax
SUM(Fact_Facturas_Lineas[Cantidad]) - SUM(Fact_Facturas_Lineas[Cantidad_Devuelta])
```

#### 90. [Importe Con IVA Facturas]
- **Carpeta:** IVA

```dax
SUM(Fact_Facturas_Lineas[Importe_Linea_ConIVA])
```

#### 91. [Importe Coste Facturas]
- **Carpeta:** Rentabilidad

```dax
SUM(Fact_Facturas_Lineas[Importe_Coste])
```

#### 92. [Importe Descuento Facturas]
- **Carpeta:** Descuentos

```dax
SUM(Fact_Facturas_Lineas[Importe_Descuento])
```

#### 93. [Importe Facturado Lineas]
- **Carpeta:** Importes

```dax
SUM(Fact_Facturas_Lineas[Importe_Linea])
```

#### 94. [Importe IVA Facturas]
- **Carpeta:** IVA

```dax
SUM(Fact_Facturas_Lineas[Importe_IVA])
```

#### 95. [Margen Bruto Facturas]
- **Carpeta:** Rentabilidad

```dax
SUM(Fact_Facturas_Lineas[Margen_Bruto])
```

#### 96. [Precio Medio Venta]
- **Carpeta:** Importes
- **Descripción:** Precio medio real de venta por unidad

```dax
DIVIDE(SUM(Fact_Facturas_Lineas[Importe_Linea]), SUM(Fact_Facturas_Lineas[Cantidad]), 0)
```

### Fact_AcuerdosGlobales_Lineas (12 medidas)

#### 97. [% Completado cantidad contrato]
- **Carpeta:** Visuales comerciales

```dax
DIVIDE ([Cantidad Servida Contrato],[Cantidad Plan Acuerdos]) 
--DIVIDE ([Cantidad Plan Acuerdos],[Cantidad Servida Contrato])
```

#### 98. [Cantidad Pendiente Servir Contrato]
- **Carpeta:** Trazabilidad contrato
- **Descripción:** Plan contractual menos cantidad ya cumplida en líneas de pedido vinculadas (Cantidad_Cumplida). Revisar si debe alinearse con Cantidad_Abierta_BA de SAP.

```dax
[Cantidad Plan Acuerdos] - [Cantidad Servida Contrato]
```

#### 99. [Cantidad Plan Acuerdos]
- **Carpeta:** Visuales comerciales
- **Descripción:** Cantidad plan en acuerdos globales.

```dax
SUM ( Fact_AcuerdosGlobales_Lineas[Cantidad_Acuerdo] )
```

#### 100. [Cantidad Servida Contrato]
- **Carpeta:** Contrato vs pedidos
- **Descripción:** Cantidad cumplida en líneas de pedido vinculadas a la línea de acuerdo por Acuerdo_Line_Key ↔ Acuerdo_Line_Key_Ref.

```dax
CALCULATE ( SUM ( Fact_Pedidos_Lineas[Cantidad_Cumplida] ), TREATAS ( VALUES ( Fact_AcuerdosGlobales_Lineas[Acuerdo_Line_Key] ), Fact_Pedidos_Lineas[Acuerdo_Line_Key_Ref] ) )
```

#### 101. [Importe Facturado Contrato]
- **Carpeta:** Trazabilidad contrato
- **Descripción:** Importe de líneas de factura enlazadas a pedidos del acuerdo (Pedido_Line_Key directo y sin doble conteo vs medidas de línea).

```dax
SUMX (
    SUMMARIZE (
        FILTER (
            ALL ( 'Fact_Pedidos_Lineas' ),
            'Fact_Pedidos_Lineas'[Acuerdo_Line_Key_Ref] IN VALUES ( 'Fact_AcuerdosGlobales_Lineas'[Acuerdo_Line_Key] )
        ),
        'Fact_Pedidos_Lineas'[Pedido_Line_Key]
    ),
    VAR k = 'Fact_Pedidos_Lineas'[Pedido_Line_Key]
    RETURN
        CALCULATE (
            SUM ( 'Fact_Facturas_Lineas'[Importe_Linea] ),
            FILTER ( ALL ( 'Fact_Facturas_Lineas' ), 'Fact_Facturas_Lineas'[Pedido_Line_Key] = k )
        )
)
```

#### 102. [Importe Pendiente Facturar Contrato]
- **Carpeta:** Trazabilidad contrato
- **Descripción:** Importe plan OOAT menos importe facturado rastreado a través de pedidos del contrato.

```dax
[Importe Plan Acuerdos] - [Importe Facturado Contrato]
```

#### 103. [Importe Plan Acuerdos]
- **Carpeta:** Visuales comerciales
- **Descripción:** Suma de importe planificado en líneas OOAT/OAT1.

```dax
BLANK()
```

#### 104. [Lista Fechas Entrega Contrato]
- **Carpeta:** Trazabilidad contrato
- **Descripción:** Lista de fechas de albarán distintas para el contrato (texto).

```dax
VAR PKset =
    SELECTCOLUMNS (
        FILTER (
            ALL ( 'Fact_Pedidos_Lineas' ),
            'Fact_Pedidos_Lineas'[Acuerdo_Line_Key_Ref] IN VALUES ( 'Fact_AcuerdosGlobales_Lineas'[Acuerdo_Line_Key] )
        ),
        "pk", 'Fact_Pedidos_Lineas'[Pedido_Line_Key]
    )
VAR DatesTbl =
    DISTINCT (
        SELECTCOLUMNS (
            FILTER (
                ALL ( 'Fact_Albaranes_Lineas' ),
                'Fact_Albaranes_Lineas'[Pedido_Line_Key] IN SELECTCOLUMNS ( PKset, "x", [pk] )
            ),
            "d", 'Fact_Albaranes_Lineas'[Fecha_Albaran]
        )
    )
RETURN
    CONCATENATEX ( DatesTbl, FORMAT ( [d], "Short Date" ), ", ", [d], ASC )
```

#### 105. [Primera Fecha Entrega Contrato]
- **Carpeta:** Trazabilidad contrato
- **Descripción:** Primera fecha de albarán vinculada a pedidos del acuerdo.

```dax
VAR PKset =
    SELECTCOLUMNS (
        FILTER (
            ALL ( 'Fact_Pedidos_Lineas' ),
            'Fact_Pedidos_Lineas'[Acuerdo_Line_Key_Ref] IN VALUES ( 'Fact_AcuerdosGlobales_Lineas'[Acuerdo_Line_Key] )
        ),
        "pk", 'Fact_Pedidos_Lineas'[Pedido_Line_Key]
    )
RETURN
    MINX (
        FILTER (
            ALL ( 'Fact_Albaranes_Lineas' ),
            'Fact_Albaranes_Lineas'[Pedido_Line_Key] IN SELECTCOLUMNS ( PKset, "x", [pk] )
        ),
        'Fact_Albaranes_Lineas'[Fecha_Albaran]
    )
```

#### 106. [Ultima Fecha Entrega Contrato]
- **Carpeta:** Trazabilidad contrato
- **Descripción:** Última fecha de albarán vinculada a pedidos del acuerdo.

```dax
VAR PKset =
    SELECTCOLUMNS (
        FILTER (
            ALL ( 'Fact_Pedidos_Lineas' ),
            'Fact_Pedidos_Lineas'[Acuerdo_Line_Key_Ref] IN VALUES ( 'Fact_AcuerdosGlobales_Lineas'[Acuerdo_Line_Key] )
        ),
        "pk", 'Fact_Pedidos_Lineas'[Pedido_Line_Key]
    )
RETURN
    MAXX (
        FILTER (
            ALL ( 'Fact_Albaranes_Lineas' ),
            'Fact_Albaranes_Lineas'[Pedido_Line_Key] IN SELECTCOLUMNS ( PKset, "x", [pk] )
        ),
        'Fact_Albaranes_Lineas'[Fecha_Albaran]
    )
```

#### 107. [importe_linea_cantidad_servida]
- **Carpeta:** Contrato vs pedidos

```dax
if([Cantidad Servida Contrato] = BLANK(),0, CALCULATE([Cantidad Servida Contrato]* SELECTEDVALUE(Fact_AcuerdosGlobales_Lineas[Precio])))
```

#### 108. [importe_linea_cantxprec]

```dax
Fact_AcuerdosGlobales_Lineas[Cantidad Plan Acuerdos] *  Fact_AcuerdosGlobales_Lineas[precio]
```

### Fact_Ofertas_Lineas (1 medidas)

#### 109. [Num Pedidos Generados desde Oferta]
- **Carpeta:** Trazabilidad oferta
- **Descripción:** Recuento de pedidos de venta con origen en la oferta (ObjectType 23=OQUT). Ampliar para intercompany cuando exista enlace compra-venta.

```dax
VAR oe = MAX ( 'Fact_Ofertas_Lineas'[DocEntry] )
RETURN
    CALCULATE (
        DISTINCTCOUNT ( 'Fact_Pedidos_Lineas'[DocEntry] ),
        FILTER (
            ALL ( 'Fact_Pedidos_Lineas' ),
            'Fact_Pedidos_Lineas'[DocOrigen_ObjectType] = 23
                && 'Fact_Pedidos_Lineas'[DocOrigen_Entry] = oe
        )
    )
```

### Fact_Inventario_Almacen (2 medidas)

#### 110. [articulos_cant_neta_insuficiente]

```dax
CALCULATE(
    COUNTROWS('Fact_Inventario_Almacen'),
    'Fact_Inventario_Almacen'[Stock_Neta_Servible] < 0
)
```

#### 111. [articulos_no_disponibles]

```dax
CALCULATE(
    COUNTROWS('Fact_Inventario_Almacen'),
    'Fact_Inventario_Almacen'[Stock_Disponible] = 0
)
```
