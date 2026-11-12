# Modelo mínimo de contribuciones académicas RIDEG · v0.1

**Estado:** propuesta técnica para revisión; no equivale al protocolo documental del XVII ni a una norma institucional adoptada.  
**Corte:** 2026-11-12. **Propósito:** registro de ponencias, conferencias, mesas, entrevistas y otros aportes con baja carga inicial.

## 1. Entidades y claves

| Entidad | Identificador de ejemplo | Uso |
|---|---|---|
| Simposio | `SIM-XVII` | Edición y año; referencia a matriz histórica |
| Sesión | `SES-XVII-001` | Mesa, panel, conferencia o actividad del programa |
| Contribución | `CON-XVII-001` | Ponencia, intervención, entrevista u otro aporte documentable |
| Evidencia | `EVD-XVII-0001` | Audio, documento, nota o fotografía: registro de original preservado |
| Institución | `INS-020` | Solo si existe identidad institucional verificada en inventario |
| Persona | `PER-00001` | Identificador editorial local; datos personales bajo protección |

La numeración es **por registro**, no por posición en el programa. Si se suspende una intervención, el identificador no se reutiliza. El ejemplo `CON-XVII-001` **no representa una ponencia real**.

## 2. Registro universal de contribuciones

Archivo modelo: `CONTRIBUCIONES_MODELO.csv`. Los **únicos campos necesarios en el instante de captura** son: `id_contribucion`, `id_simposio`, `tipo_contribucion`, `estado_registro` y `nota_captura` (puede ser mínima). Fecha, hora y sesión son recomendables cuando se conocen; no se inventan.

| Campo | Descripción | Captura |
|---|---|---|
| id_contribucion | Clave estable | Generar una vez |
| id_simposio | Edición | Elegir |
| id_sesion | Relación con programa | Opcional, posteriormente conciliable |
| tipo_contribucion | ponencia / conferencia / entrevista / mesa / otro | Elegir |
| titulo_literal | Título como figura en fuente; vacío hasta cotejo | Posterior |
| momento_local | ISO 8601 con huso horario cuando se dispone | Automático o posterior |
| estado_registro | planificado / capturado / cancelado / sustituido | Elegir |
| nota_captura | Observación factual breve | Captura |
| fuente_programa | ID o ruta del documento fuente | Precarga |
| observaciones | Dudas, discrepancias, contexto | Posterior |

Para evitar nombres duplicados y errores de transcripción, **las autorías, afiliaciones y evidencias se registran como relaciones separadas**, no como texto incrustado en la ficha.

## 3. Relaciones

Archivo modelo: `RELACIONES_MODELO.csv`. Cada fila es un vínculo afirmado con su propia evidencia y estado.

| Campo | Significado |
|---|---|
| id_relacion | ID único de la relación |
| origen_tipo / origen_id | Ej.: contribucion / CON-XVII-001 |
| relacion | ocurrió_en / tiene_evidencia / atribuido_a / afiliacion_declarada / organizado_por |
| destino_tipo / destino_id | Ej.: sesión / SES-XVII-001 |
| fuente_id | Fuente que sustenta el vínculo |
| estado_verificacion | referenciado / capturado / revisado / verificado |
| nota | Cita localizable o incertidumbre |

Reglas: **autor/a ≠ institución**, **institución de afiliación ≠ sede**, **ponencia en programa ≠ ponencia efectivamente presentada**, **declaración propuesta ≠ acuerdo adoptado**. Una relación sin fuente se registra como **pendiente de verificación**, nunca como hecho confirmado.

## 4. Evidencia y permiso de difusión

Archivo modelo: `EVIDENCIAS_MODELO.csv`. La **evidencia** y la **contribución** pueden tener relación de uno a muchos (por ejemplo, audio + nota). Mantener originales fuera del repositorio público.

| Campo | Descripción |
|---|---|
| id_evidencia | Clave estable |
| tipo_evidencia | audio / imagen / nota / pdf / otro |
| ubicacion_custodia | Ruta relativa o referencia segura, **sin publicar ubicaciones sensibles** |
| sha256 | Se añade al importar o consolidar original, no durante captura a mano |
| estado_verificacion | referenciado / capturado / revisado / verificado |
| autorizacion_publicacion | no_evaluada / restringida / autorizada |
| fuente_autorizacion | ID del consentimiento o autorización bajo custodia privada, si corresponde |

**Verificado no significa autorizado.** No subir audios, consentimientos, datos de contacto personales ni imágenes identificables sin revisar finalidad, permisos y derecho aplicable.

## 5. Estados: dos dimensiones independientes

**Calidad de evidencia**: `referenciado` (se conoce una referencia) → `capturado` (se conserva una copia o nota original) → `revisado` (comprobación humana) → `verificado` (contraste suficiente de contenido y atribución). No todos los registros tendrán que alcanzar la última etapa inmediatamente.

**Difusión**: `no_evaluada` / `restringida` / `autorizada`. No se asume autorización por ser evento público o por figurar en el programa.

Los cambios de estado deben quedar documentados con versión, persona responsable cuando corresponda, fecha y fundamento; los CSV iniciales son **plantillas**, no historiales de aprobación.

## 6. Regla de operación mínima

1. **Antes:** precargar edición, sesiones, títulos y nombres **desde el programa**, marcándolos `planificado` o `referenciado`.
2. **Durante:** elegir sesión/contribución, registrar inicio/nota y evidencia; marcar `capturado` cuando efectivamente se conservó.
3. **Después:** revisar nombre, atribución y archivo; calcular SHA-256; enlazar fuentes; revisar permisos.
4. **Publicación:** decisión editorial separada; la memoria o declaración final no hereda automáticamente estados de borradores.

**No se incluyen herramientas de automatización ni captura de datos reales en esta fase.** Se revisarán cuando se aporte el protocolo de entrevista y programa XVII.
