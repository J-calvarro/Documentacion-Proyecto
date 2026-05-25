# Anexo — Diccionario de columnas del modelo `Estructura_AGRU_PRUEBA_v3`

Exportado desde el modelo semántico (Power BI Desktop).  
Columnas técnicas `RowNumber-*` omitidas (clave interna Power BI).

**Leyenda origen:** `SAP` = columna física en ETL; `DAX` = columna calculada en el modelo; `SQL` = derivada en procedimiento de carga.

---

## Fact_AccumSnapshot_Pedidos (29 columnas · 1 fila/pedido)

| Campo | Tipo | Origen SAP / lógica |
|-------|------|---------------------|
| DocEntry | Int64 | ORDR.DocEntry (PK) |
| DocNum | Int64 | ORDR.DocNum |
| CardCode | String | ORDR.CardCode → Dim_Cliente |
| CardName | String | ORDR / OCRD |
| SlpCode | Int64 | ORDR.SlpCode → Dim_Vendedor |
| Fecha_Pedido | DateTime | ORDR.DocDate |
| Fecha_Creacion | DateTime | ORDR.CreateDate |
| Fecha_VencimientoPedido | DateTime | ORDR.DocDueDate |
| Fecha_EntregaSolicitada | DateTime | ORDR.ReqDate |
| Fecha_Entrega | DateTime | MIN(ODLN.DocDate) — relación activa Dim_Fecha |
| Fecha_Factura | DateTime | MIN(OINV.DocDate) — relación inactiva |
| Fecha_Cobro | DateTime | ORCT / pagos — relación inactiva |
| Importe_Pedido | Double | ORDR.DocTotal / suma líneas |
| Importe_Facturado | Double | Agregado facturas |
| Importe_Cobrado | Double | Agregado cobros |
| Moneda | String | ORDR.DocCur |
| Estado_Pedido | String | ORDR.DocStatus |
| Cancelado | String | ORDR.CANCELED (Y/N) |
| Num_Entregas | Int64 | Conteo ODLN |
| Num_Facturas | Int64 | Conteo OINV |
| Etapa_Actual | String | 1-Pedido … 4-Cobrado (SQL/DAX) |
| Dias_Pedido_a_Entrega | Int64 | DATEDIFF pedido→entrega |
| Dias_Entrega_a_Factura | Int64 | DATEDIFF entrega→factura |
| Dias_Factura_a_Cobro | Int64 | DATEDIFF factura→cobro (DSO) |
| Dias_Ciclo_Acumulado | Int64 | Ciclo total acumulado |
| Dias_Retraso_Entrega | Int64 | vs Fecha_EntregaSolicitada |
| Flag_Entregado | Int64 | 0/1 hito entrega |
| Flag_Facturado | Int64 | 0/1 hito factura |
| Flag_Cobrado | Int64 | 0/1 hito cobro |

---

## Fact_Pedidos_Lineas (47 columnas · ORDR+RDR1)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| DocEntry | Int64 | ORDR.DocEntry |
| LineNum | Int64 | RDR1.LineNum |
| DocNum | Int64 | ORDR.DocNum |
| CardCode | String | ORDR.CardCode |
| SlpCode | Int64 | ORDR.SlpCode |
| Fecha_Pedido | DateTime | ORDR.DocDate |
| Fecha_Vencimiento | DateTime | ORDR.DocDueDate |
| Fecha_Entrega_Solicitada | DateTime | RDR1.ShipDate |
| ItemCode | String | RDR1.ItemCode |
| Descripcion | String | RDR1.Dscription |
| Cantidad | Double | RDR1.Quantity |
| Cantidad_Pendiente | Double | RDR1.OpenQty |
| Cantidad_Cumplida | Double | Derivado entregas SAP |
| Cantidad_Inventario | Double | RDR1.InvQty |
| Importe_Linea | Double | RDR1.LineTotal |
| Precio_Tarifa | Double | RDR1.PriceBefDi |
| Precio_Neto | Double | RDR1.Price |
| Descuento_Pct | Double | RDR1.DiscPrcnt |
| Importe_Descuento | Double | Calculado |
| IVA_Pct | Double | RDR1.VatPrcnt |
| Importe_IVA | Double | RDR1.VatSum |
| Importe_Linea_ConIVA | Double | Calculado |
| Precio_Coste | Double | RDR1.INMPrice / coste |
| Importe_Coste | Double | Calculado |
| Margen_Bruto | Double | Importe − coste |
| Margen_Bruto_Pct | Double | % margen |
| Moneda | String | ORDR.DocCur |
| Almacen | String | RDR1.WhsCode |
| Estado_Linea | String | RDR1.LineStatus O/C |
| Estado_Pedido | String | ORDR.DocStatus |
| Codigo_IVA | String | RDR1.TaxCode |
| Estado_Picking | String | RDR1.PickStatus |
| Ref_Cliente | String | ORDR.NumAtCard |
| Proyecto | String | RDR1.Project |
| Centro_Coste | String | RDR1.OcrCode |
| Comentarios | String | ORDR.Comments |
| Pedido_Line_Key | String | **DAX:** FORMAT(DocEntry)&"_"&FORMAT(LineNum) |
| Id_Sucursal | Int64 | ORDR.BPLId |
| Nombre_Sucursal | String | OBPL.BPLName |
| AgrNo_Acuerdo_OOAT | Int64 | RDR1.AgrNo |
| AgrLnNum_Acuerdo | Int64 | RDR1.AgrLnNum |
| Numero_Acuerdo_Global | Int64 | OOAT |
| Acuerdo_Fecha_Inicio | DateTime | OOAT |
| Acuerdo_Fecha_Fin | DateTime | OOAT |
| Acuerdo_Line_Key_Ref | String | Enlace OOAT/OAT1 |
| DocOrigen_Entry | Int64 | RDR1.BaseEntry / cabecera |
| DocOrigen_ObjectType | Int64 | RDR1.BaseType (23=oferta, etc.) |

---

## Fact_Albaranes_Lineas (40 columnas · ODLN+DLN1)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| DocEntry, LineNum, DocNum | Int64 | ODLN / DLN1 |
| CardCode, SlpCode | String/Int64 | ODLN |
| Fecha_Albaran | DateTime | ODLN.DocDate |
| ItemCode, Descripcion | String | DLN1 |
| Cantidad, Importe_Linea | Double | DLN1 |
| Pedido_DocEntry, Pedido_LineNum | Int64 | DLN1.BaseEntry, BaseLine (BaseType 17) |
| Tipo_Origen | Int64 | DLN1.BaseType |
| Albaran_Line_Key | String | **DAX:** DocEntry_LineNum |
| Pedido_Line_Key | String | **DAX:** desde Pedido_DocEntry+LineNum |
| Peso_Line_Kg, Volumen_Line | Double | DLN1.Weight1, Volume |
| Fecha_Carga_Line | DateTime | DLN1.ShipDate |
| Id_Sucursal, Nombre_Sucursal | Int64/String | ODLN.BPLId / OBPL |
| (+ campos rentabilidad/IVA análogos a pedidos) | | DLN1 |

---

## Fact_Facturas_Lineas (43 columnas · OINV+INV1)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| DocEntry, LineNum, DocNum | Int64 | OINV / INV1 |
| Fecha_Factura | DateTime | OINV.DocDate |
| Fecha_Vencimiento_Pago | DateTime | OINV.DocDueDate |
| Fecha_Devengo | DateTime | OINV.TaxDate |
| Albaran_DocEntry, Albaran_LineNum | Int64 | INV1.BaseEntry, BaseLine (15) |
| Cantidad_Devuelta | Double | Agregado devoluciones |
| Importe_Pagado | Double | OINV.PaidToDate (prorrateo línea) |
| Importe_Pendiente_Cobro | Double | Calculado |
| Estado_Factura | String | OINV.DocStatus |
| Factura_Line_Key | String | **DAX:** DocEntry_LineNum |
| Albaran_Line_Key | String | **DAX:** si BaseType=15 |
| Pedido_Line_Key | String | **DAX:** si BaseType=17 |
| (+ rentabilidad, IVA, trazabilidad) | | INV1 |

---

## Fact_Ofertas_Lineas (26 columnas · OQUT+QUT1)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| Oferta_Line_Key | String | SQL/DAX clave compuesta |
| DocEntry, LineNum, DocNum | Int64 | OQUT / QUT1 |
| Fecha_Oferta, Fecha_Validez | DateTime | OQUT |
| Cantidad, Cantidad_Abierta | Double | QUT1 |
| Estado_Oferta, Estado_Linea | String | OQUT / QUT1 |
| DocOrigen_Entry, DocOrigen_ObjectType | Int64 | Trazabilidad |
| Id_Sucursal, Nombre_Sucursal | Int64/String | OQUT.BPLId |

---

## Fact_AcuerdosGlobales_Lineas (16 columnas · OOAT+OAT1)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| Acuerdo_Line_Key | String | AgrNo + AgrLnNum |
| Numero_Acuerdo | String | OOAT |
| CardCode | String | OOAT.BpCode |
| Fecha_Inicio, Fecha_Fin | DateTime | OOAT |
| Estado_Acuerdo | String | OOAT.Status |
| LineNum | Int64 | OAT1 |
| ItemCode, Descripcion_Articulo | String | OAT1 |
| Cantidad_Acuerdo | Double | OAT1.PlanQty |
| Cantidad_Abierta_BA | Double | OAT1.UndlvQty |
| Precio | Double | OAT1.UnitPrice |
| Importe_Line | Double | OAT1 |
| Acuerdo_AbsID | Int64 | OOAT.AbsID |
| Nombre_Interlocutor | String | OOAT.BpName |
| importe_linea | Double | **DAX:** Cantidad × Precio |

---

## Fact_Devoluciones_Lineas (20 columnas · ORDN+RDN1)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| Devolucion_Line_Key | String | Clave compuesta |
| DocEntry, LineNum, DocNum | Int64 | ORDN / RDN1 |
| Fecha_Devolucion | DateTime | ORDN.DocDate |
| DocOrigen_Entry, DocOrigen_ObjectType, DocOrigen_Line | Int64 | RDN1.Base* (17=pedido) |
| Cantidad, Importe_Linea | Double | RDN1 |
| Id_Sucursal, Nombre_Sucursal | Int64/String | ORDN.BPLId |

---

## Fact_Abonos_Lineas, Fact_PedidosCompra_Lineas, Fact_Solicitudes_Devolucion_Lineas

Estructura análoga a devoluciones/facturas: `DocEntry`, `LineNum`, `CardCode`, `ItemCode`, `Cantidad`, `Importe_Linea`, `DocOrigen_*`, `Id_Sucursal`.  
Origen SAP: **ORIN+RIN1** (abonos, ObjType 14), **OPOR+POR1** (compras, 22), **ORRR+RRR1** (solicitudes devolución).

---

## Fact_Inventario_Almacen (6 columnas · OITW+OITM)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| ItemCode | String | OITW.ItemCode |
| Almacen | String | OITW.WhsCode |
| Stock_Disponible | Double | OITW.OnHand |
| Stock_Comprometido | Double | OITW.IsCommited |
| Stock_Pedido_Compra | Double | OITW.OnOrder |
| Stock_Neta_Servible | Double | SQL: OnHand − IsCommited (+ reglas negocio) |

---

## Dim_Cliente (11 columnas · OCRD)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| CardCode | String | OCRD.CardCode (único) |
| Nombre | String | OCRD.CardName |
| GrupoCliente | Int64 | OCRD.GroupCode |
| Telefono | String | OCRD.Phone1 |
| Contacto | String | OCRD.CntctPrsn |
| Ciudad, Pais, CodigoPostal | String | OCRD |
| Email | String | OCRD.E_Mail |
| DefaultSlpCode | Int64 | OCRD (vendedor por defecto) |

---

## Dim_Vendedor (4 columnas · OSLP)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| SlpCode | Int64 | OSLP.SlpCode |
| Vendedor | String | OSLP.SlpName |
| Notas | String | OSLP.Memo |
| Activo | String | OSLP.Active |

---

## Dim_Producto (10 columnas · OITM)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| ItemCode | String | OITM.ItemCode |
| Nombre | String | OITM.ItemName |
| GrupoArticulo | String | OITB vía ItmsGrpCod |
| TipoArticulo | String | OITM.ItemType |
| EsInventariable, EsVendible | String | OITM.InvntItem, SellItem |
| PrecioMedio | Double | OITM.AvgPrice |
| StockActual, StockComprometido | Double | OITM.OnHand, IsCommited |

---

## Dim_Fecha (16 columnas · calendario)

| Campo | Tipo | Origen |
|-------|------|--------|
| Date | DateTime | Tabla calendario generada |
| Año, NroTrimestre, Trimestre, AñoTrimestre | Int64/String | Derivados |
| NroMes, Mes, MesCorto, AñoMes, AñoMesTexto | — | Derivados |
| Semana, DiaSemana, NomDia, DiaMes | — | Derivados |
| EsFinDeSemana | Int64 | Derivado |
| Periodo | String | Derivado |

Jerarquía: **Año → Mes → DiaMes**.

---

## Dim_Sucursal (2 columnas · OBPL)

| Campo | Tipo | Origen SAP |
|-------|------|------------|
| Id_Sucursal | Int64 | OBPL.BPLId |
| Nombre_Sucursal | String | OBPL.BPLName |

---

## Tabla_Filtro_Cobertura (desconectada)

| Campo | Tipo | Uso |
|-------|------|-----|
| Etiqueta | String | Valores: Sin pendiente, Stock suficiente, Stock insuficiente — filtro visual vía medida `Filtrar por Cobertura` |
