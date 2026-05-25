# Anexo — Catálogo completo `stage.TableList` (106 tablas)

**Base de metadatos ETL:** `AETL_SBOBI_v2.stage.TableList`  
**Plantilla:** `CodEmpresa = -1`  
**Fuente:** `table_list_24_04_26.sql` + actualizaciones en `INSTRUCCIONES_TABLELIST_UPDATE_INSERT.txt`  
**Frecuencia de sincronización:** diaria (junto con el job ETL principal)

> Cada fila define `SourceColumns` = `DestinationColumns` (misma lista, mismo orden).  
> `CompleteLoad = 1` en todas las entradas de la plantilla.  
> Destino stage: `SAP_STGA*F.dbo.<Tabla>` con columna `CodEmpresa`.

---

## Índice por dominio

### Maestros y configuración
| Tabla | Nº col. | Columnas (resumen) |
|-------|---------|-------------------|
| OBPL | 4 | CodEmpresa, BPLId, BPLName, Disabled |
| OCRD | 52 | CardCode, CardName, GroupCode, SlpCode, …, CntctPrsn |
| OITM | 68 | ItemCode, ItemName, atributos U_AGR_*, OnHand, validFor, … |
| OSLP | 16 | SlpCode, SlpName, Memo, Commission, Active, Email, … |
| OITW | 6 | ItemCode, WhsCode, OnHand, IsCommited, OnOrder, updateDate |
| OITB | 68 | Grupos de artículos y cuentas contables |
| OWHS | 3 | WhsCode, WhsName, Location |
| OCRG | 9 | Grupos de socios de negocio |
| OCRY / OCST | País y provincias |
| OCTG | Condiciones de pago |
| OUGP / UGP1 / OUOM | Unidades de medida |
| OADM | 2 | Code, ContInvnt |
| CUFD / UFD1 | Campos definidos por usuario |
| @AGR_COMERCIALTEC | 2 | Code, Name |
| @AGR_TIPOPRODUCCION | 2 | Code, Name |
| @AGR_LINEAPRODUCCION | 2 | Code, Name |

### Ventas — cabeceras de documento
| Tabla | Documento SAP | Campos destacados |
|-------|---------------|-------------------|
| ORDR | Pedido venta | DocEntry, DocNum, CardCode, DocDate, BPLId, U_AGR_*, DocTotal, ReqDate, CreateDate |
| ODLN | Albarán | DocEntry, DocNum, CardCode, DocDate, BPLId, U_AGR_* |
| OINV | Factura | DocEntry, DocNum, DocTotal, PaidToDate, TaxDate, BPLId |
| OQUT | Oferta | DocEntry, DocNum, U_AGR_* |
| ORDN | Devolución | Similar a ORDR |
| ORIN | Abono / nota crédito | TaxDate, Comments, BPLId |
| ORRR | Solicitud devolución | U_AGR_*, Comments |
| OOAT | Acuerdo global | Status, BpCode, fechas, BpName |

### Ventas — líneas de documento
| Tabla | Líneas | Campos destacados |
|-------|--------|-------------------|
| RDR1 | Pedido | DocEntry, LineNum, Quantity, OpenQty, BaseEntry, BaseType, U_AGR_* línea, GrossBuyPr, GrssProfit |
| DLN1 | Albarán | + DiscPrcnt, Dscription, Volume, TrgetEntry |
| INV1 | Factura | + InvQty, Price, Currency, GrossBuyPr, GrssProfit |
| QUT1 | Oferta | + OcrCode, TaxCode |
| RDN1 | Devolución | + Dscription |
| RIN1 | Abono | + DiscPrcnt, InvQty, Price, Currency |
| RRR1 | Solic. devolución | + Dscription |
| OAT1 | Acuerdo (líneas) | AgrNo, PlanQty, UnitPrice, UndlvQty, … |

### Compras
| Tabla | Documento |
|-------|-----------|
| OPOR / POR1 | Pedido de compra |
| OPQT / PQT1 | Oferta de compra |
| OPCH / PCH1 | Factura compra |
| OPDN / PDN1 | Entrada mercancía compra |

### Finanzas y cobros
| Tabla | Uso |
|-------|-----|
| ORCT / RCT2 | Cobros y aplicación a facturas |
| OBOE / BOT1 | Efectos / letras de cambio |
| INV6 / RIN6 | Vencimientos de factura/abono |
| OJDT / JDT1 | Asientos contables |
| OVPM / VPM2 | Pagos salientes |

### Inventario y costes
| Tabla | Uso |
|-------|-----|
| OINM | Movimientos de inventario |
| OITL / ITL1 | Trazabilidad lotes |
| OBTN / OBTQ / ABTN | Lotes y stock por lote |
| @IFG_PMC | Precio medio de coste |
| @IFG_COSTESVENTA_CAB / _LIN | Costes de venta |

### Producción
| Tabla | Uso |
|-------|-----|
| OWOR / WOR1 / WOR2 / WOR4 | Órdenes de fabricación |
| OITT / ITT1 | Estructuras de producto |
| OIGN / IGN1 / IGE1 | Entradas/salidas inventario |

### Listado alfabético de las 106 tablas

ABTN, BOT1, CRD1, CRD3, CUFD, DLN1, DSC1, IGE1, INV1, INV6, ITL1, ITM12, ITM4, ITT1, JDT1, NNM1, OACT, OADM, OAGP, OBGS, OBOT, OBTN, OBTQ, OBPL, OCCT, OCOG, OAT1, OCRB, OCRD, OCRG, OCRY, OCTG, ODLN, ODIM, ODSC, OFPR, OIGN, OINV, OIPF, IPF1, OITB, OITL, OITT, OITM, OITW, OJDT, OLCT, OMRC, OOAT, @AGR_COMERCIALTEC, OOCR, OPCH, OPDN, OPOR, OPQT, OPRC, OPRJ, OPYM, OQUT, ORCT, ORDN, ORDR, ORIN, OUGP, OVPM, OWHS, OWOR, OTER, @AGR_LINEAPRODUCCION, PCH1, PDN1, POR1, PQT1, QUT1, RAC, RCT2, RDN1, RDR1, RIN1, RIN3, RIN6, RPC1, RPD1, RRR1, RRR21, UFD1, UGP1, VPM2, WOR1, WOR2, @AGR_TIPOPRODUCCION, @IFG_COSTESVENTA_CAB, @IFG_COSTESVENTA_LIN, @IFG_PMC

---

## Tablas con actualización incremental documentada (24/04/2026)

Según `INSTRUCCIONES_TABLELIST_UPDATE_INSERT.txt`, estas tablas recibieron ampliación de columnas en TableList:

DLN1, INV1, OCRD, ODLN, OINV, OITM, OOAT, OPOR, OQUT, ORDN, ORDR, ORIN, ORRR, POR1, QUT1, RDN1, RDR1, RIN1, RRR1, OBPL (INSERT nuevo)

Para el detalle columna a columna de cada tabla, consultar las sentencias `INSERT`/`UPDATE` en los archivos SQL del directorio `AGRUCAPERS`.
