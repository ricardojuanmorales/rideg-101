# Registro AHE | Preparación editorial del lote consolidado de 21 documentos

**Fecha:** 2026-11-15  
**Proyecto:** RIDEG 101 · XVII Simposio Internacional de Estudios Generales  
**Estado:** DECLARACIÓN HUMANA RECIBIDA; PREPARACIÓN TÉCNICA COMPLETADA; PUBLICACIÓN COMPLETA NO EJECUTADA; VALIDACIÓN EDITORIAL PENDIENTE.  
**PR de seguimiento:** #14, abierto en borrador. **Arquitectura:** PR #17, fusionado.

## Declaración del responsable

En la conversación del proyecto, la persona responsable afirmó:

> «AHE: Declaro que cuento con autorización para publicar los 21 documentos consolidados del XVII Simposio RIDEG. Procede a verificar el alcance y evidencia de los permisos y prepara la integración bajo revisión humana.»

Se registra como **declaración expresa de autorización del responsable del proyecto** para el lote delimitado de 21 documentos. No se adjuntaron en la conversación instrumentos de consentimiento, licencias, autorizaciones de los titulares de derechos ni constancias específicas de difusión de aportes de terceros. Por lo tanto, **la comprobación documental independiente de esos permisos no está acreditada**. No se inventarán evidencias ni se marcarán como verificadas.

## Alcance del lote aprobado por declaración

- **21 documentos únicos:** 16 reportes de contribuciones CON, 1 relatoría SES-XVII-02, 1 investigación transversal UPR-INTEC-UNSA, 1 entrevista académica, 1 prospectiva del XVIII Simposio y 1 reporte del cierre del XVII.
- **16 códigos CON:** 006, 007, 009, 010, 011, 012, 013, 014, 015, 016, 022, 023, 024, 025, 026 y 033 (prefijo CON-XVII-).
- **Exclusiones:** duplicado binario CON-XVII-011, ficheros auxiliares macOS, las demás contribuciones no presentes en el ZIP y documentos de terceros que no formen parte de este lote.
- **ZIP de origen SHA-256:** `2d9a3d480f44775df099e6240c9613d848d4efe355f0a0b4ccd600e77fbecfe4`.
- **ZIP de preparación para revisión SHA-256:** `3b0bf3a9d1120da224f28a24f1d9e69166854c8fc4187163c05097defe29d995`.
- **Comprobación técnica:** 21 hashes de documentos en el paquete de preparación coinciden con el manifiesto de procedencia; 33 archivos en el ZIP (21 documentos y 12 archivos auxiliares README/control). No se alteraron los bytes de los 21 documentos recibidos.

## Clasificación editorial

La autorización declarada para publicar los textos **no acredita por sí sola** verificación de citas, exactitud de transcripción, aprobación individual de terceros, ni validez de los análisis. Los textos son reportes académicos analíticos preparados por RIDEG 101, no necesariamente manuscritos originales revisados por cada ponente.

**Excepciones que deben quedar visibles en la revisión:**
- La entrevista `RIDEG101_Entrevista_Gualdemiro_Velez_Reporte_Final.md` declara expresamente pendiente la validación de la persona entrevistada.
- Diversos reportes utilizan títulos analíticos reconstruidos o provisionales; no reemplazar los títulos oficiales del programa sin cotejo.
- Se reconocen límites de transcripciones orales, referencias sin verificar y análisis interpretativos. La agenda acredita programación, no prueba por sí sola ejecución.
- La existencia de autorización de difusión no equivale a autorización para atribuir al ponente la autoría editorial del reporte analítico.

## Preparación técnica y destino propuesto

Se creó un **único paquete ZIP local de carga Git-ready** con rutas por función primaria y un `MANIFIESTO_AHE_21_DOCUMENTOS.csv` que identifica por archivo: ruta, SHA-256, tamaño, tipo, origen, declaración AHE y estado de verificaciones. No contiene datos agregados a los documentos académicos originales. La estructura propone corpus CON en 13, relatorías en síntesis, entrevista como fuente, investigación transversal como análisis, prospectiva en 14 y cierre de evento en 18; estas rutas aún requieren revisión semántica definitiva.

**Importante:** no se subió ZIP ni los 21 Markdown completos a GitHub en este registro. Como GitHub es público, incluso un PR en borrador publicaría íntegramente su contenido. El paquete se mantiene como artefacto descargable de custodia y preparación editorial.

## Controles previos a publicar íntegramente

1. Conservar evidencia de alcance de los permisos aplicables a los 21 archivos o aceptación institucional documentada de la responsabilidad editorial; identificar restricciones individuales.
2. Confirmar si la entrevista puede difundirse como reporte sin validación del entrevistado y describirla de forma inequívoca.
3. Verificar que rutas propuestas no colisionen con documentos existentes y que la distinción entre reportes RIDEG 101 y textos de ponentes sea visible.
4. Registrar manifiesto definitivo y resultado de la revisión humana del PR.
5. Tras evidencia suficiente, incorporar en bloque al PR #14, sin merge automático; solicitar nueva autorización humana para integración a `main`.

## Secuencia posterior

Publicación controlada del lote que supere los controles → revisión del PR #14 → autorización humana del merge → pruebas de integridad/navegación y primera versión funcional → actualización del README público con el estado real.
