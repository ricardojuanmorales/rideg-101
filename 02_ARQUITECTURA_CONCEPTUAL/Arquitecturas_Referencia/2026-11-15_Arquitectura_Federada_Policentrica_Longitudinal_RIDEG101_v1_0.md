# RIDEG 101 | Arquitectura federada policéntrica longitudinal v1.0

**Fecha de decisión humana:** 2026-11-15  
**Estado de decisión:** APROBADO para aplicación piloto controlada en el XVII Simposio RIDEG.  
**Estado de implementación:** PENDIENTE de validación empírica mediante el corpus; aprobación conceptual no equivale a certificación técnica ni editorial.  
**Ruta canónica:** `02_ARQUITECTURA_CONCEPTUAL/Arquitecturas_Referencia/`  
**Naturaleza:** arquitectura de referencia de RIDEG 101, compatible con el Framework Genérico; no sustituye su canon ni altera automáticamente otras decisiones.  
**Expediente de aprobación:** `18_DOCUMENTACION_ACTIVA/Registro_Decisiones/2026-11-15_Decision_Arquitectura_Federacion_Policentrica_RIDEG101_v1_0.md`

## 1. Propósito y alcance

Organizar la memoria histórica viva y el conocimiento académico de la Red Internacional de Estudios Generales sin subsumir los actores, fuentes, currículos, conceptos y obras en los simposios. Permitir investigación longitudinal, comparativa, bibliográfica, curricular, filosófica, transdisciplinaria, pedagógica e institucional. El XVII Simposio (Arequipa, 12–14 de noviembre de 2026) será el primer caso de aplicación y validación, no el límite de la arquitectura.

## 2. Principios aprobados

1. **Federación policéntrica:** los simposios son acontecimientos articuladores, no propietarios de las identidades intelectuales e institucionales.
2. **Una fuente canónica, múltiples referencias lógicas:** cada objeto documental íntegro reside una sola vez. Los índices y vistas no constituyen duplicados.
3. **Residencia por función primaria:** la antigüedad, formato o tema no determinan por sí solos el cartapacio; respetar 00–21 + 99 y aprovechar familias existentes.
4. **Distinción epistemológica:** fuente/evidencia, interpretación, decisión y canon no son equivalentes; toda inferencia conserva procedencia y grado de verificación.
5. **Temporalidad longitudinal:** separar fecha del hecho, periodo de vigencia, registro, verificación y revisión.
6. **Identidad y atribución autónomas:** autoría, filiación, documento, contribución, memoria y versión no se confunden.
7. **Evolución sin borrado:** preservar divergencias, estados anteriores, conflictos, faltantes y relaciones de sustitución.
8. **Interoperabilidad:** extender el Contrato de Base de Conocimiento Común V5 existente, sin crear una segunda base monolítica ni renumerar identificadores históricos.
9. **Privacidad, derechos y permisos:** GitHub público, ramas y PR públicos no son espacios privados; no publicar contenidos completos sin difusión autorizada.
10. **Aprobación Humana Expedita (AHE):** aprobar operaciones delimitadas por manifiesto, con excepciones y reversibilidad; no sustituye la verificación de derechos ni la aprobación explícita del merge.

## 3. Dominios de conocimiento

- **Acontecimientos y gobernanza:** simposios, sesiones, actas, declaraciones, convocatorias, acuerdos, decisiones.
- **Actores y comunidades:** personas, instituciones, unidades académicas, redes, participaciones y afiliaciones fechadas.
- **Producción intelectual:** contribuciones, memorias que las documentan, obras, referencias, proposiciones y conceptos.
- **Educación y currículo:** programas, mapas curriculares versionados, cursos, competencias, prácticas y evidencias de aprendizaje.
- **Investigación y síntesis:** fuentes, métodos de examen, críticas, relatorías, análisis comparativos y hallazgos longitudinales.

Estas son familias semánticas, no nuevos cartapacios raíz.

## 4. Entidades mínimas y extensibles

| Entidad | Clave propuesta o existente | Regla |
|---|---|---|
| Evento | `SIM-XVII` | Conserva edición, fecha, sede, modalidad y fuentes |
| Sesión | `SES-XVII-XX` | Se vincula con evento; no equivale a contribución |
| Contribución | `CON-XVII-XXX` | Identidad intelectual separada de su memoria |
| Persona | `PER-XXXX` (candidato) | No inferir identidad ni afiliación sin evidencia |
| Institución | `INS-XXXX` (candidato) | Nombre normalizado y denominación histórica |
| Documento/manifestación | `DOC-XXXX` (candidato) | Tipo, fuente, formato, ubicación/custodia, hash y versión |
| Obra o referencia | `REF-XXXX` (candidato) | Desambiguar obra, edición, cita y aparición bibliográfica |
| Concepto | `CPT-XXXX` (candidato) | Definiciones atribuidas y disputas, no consenso impuesto |
| Currículo | `CUR-XXXX` (candidato) | Institución, programa, versión y vigencia |
| Competencia | `CMP-XXXX` (candidato) | Formulación, contexto y evidencia |
| Acuerdo | `ACU-XXXX` (candidato) | Acta/declaración, fecha, texto y estado de seguimiento |
| Investigación/análisis | `INV-XXXX` (candidato) | Método, corpus, inferencias y limitaciones |

Los prefijos nuevos NO están aún activados. Antes de asignarlos masivamente, cotejar convenciones y esquemas V5 y resolver colisiones; preservar identificadores existentes, incluido `BA-003` conflictivo señalado en la migración previa.

## 5. Relaciones tipadas

Relaciones iniciales: `forma_parte_de`, `documenta`, `tiene_autoria`, `afiliado_a`, `participa_en`, `cita`, `desarrolla`, `contrasta_con`, `implementa`, `aprueba`, `sustituye`, `deriva_de` y `respalda`.

Cada relación sustantiva debe vincular origen, predicado, destino, fuente/fragmento o página cuando exista, periodo, estado de verificación e identificación de la interpretación. Una relación inferida nunca se presentará como hecho documental. El modelo de relación se puede implantar inicialmente en CSV y posteriormente exportarse a JSON/grafo.

## 6. Orientación canónica por función

| Familia | Residencia preferente |
|---|---|
| Reglas, esquemas, índices maestros y ubicación | `00_CONTROL_MAESTRO/` |
| Fundamentos epistemológicos y filosóficos | `01_FUNDAMENTO_FILOSOFICO/` |
| Arquitectura conceptual, ontologías y mapas | `02_ARQUITECTURA_CONCEPTUAL/` |
| Metodologías reproducibles | `03_METODOLOGIA_Y_FLUJO_DE_TRABAJO/` |
| Competencias y taxonomías formativas | `05_COMPETENCIAS_Y_PERFILES/` |
| Programas, currículos y trayectorias | `08_CURSOS_PROGRAMAS_Y_TRAYECTORIAS/` |
| Corpus de investigación, fuentes, crítica, bibliografía y análisis | `13_INVESTIGACION_Y_EVIDENCIA/` |
| Directorio, comunidad y transferencia institucional | `14_COMUNIDAD_TRANSFERENCIA_Y_ESCALAMIENTO/` |
| Cooperación internacional y adaptación contextual | `17_INTERNACIONALIZACION_LOCALIZACION/` |
| Agenda, cobertura, recepción y trabajo en curso | `18_DOCUMENTACION_ACTIVA/` |
| Navegación humana e índices de consulta | `21_WIKI_DOCUMENTACION_HUMANA/` |
| Releases, versiones retiradas, paquetes y ciclos archivados | `99_ARCHIVO_HISTORICO/` |

**Límite de 13:** no almacenar por defecto toda la historia, perfiles institucionales, currículos y conceptos filosóficos; alojar solo objetos cuya función primaria sea investigativa.  
**Límite de 99:** no mover fuentes por su antigüedad ni duplicar todo simposio; reservar para la función archivística y cierres/versiones pertinentes.  
**Actas y declaraciones:** constituyen documentos primarios con identidad propia, custodia y referencias; su ubicación física definitiva se decidirá por residencia semántica y permisos, no por trasladarlos automáticamente a `99`.  
**Expediente de simposio:** índice lógico persistente que enlaza documentos y entidades con sus rutas canónicas, no una copia del corpus.

No crear subcarpetas o nuevas jerarquías por tema sin verificar primero las rutas existentes y registrar una decisión estructural.

## 7. Contrato mínimo de registro

Para cada objeto: `id`, `tipo`, `nombre/titulo`, `procedencia`, `fuente`, `ruta_canonica_o_custodia`, `estado_documental`, `verificacion`, `difusion`, `fechas_relevantes` y `relaciones`. Para archivos recibidos: `sha256`, tamaño y nombre original; para cambios editoriales: versión, transformación y trazabilidad.

Distinguir cuatro estados: documental (recibido/final/sustituido), verificación (pendiente/parcial/verificado/observado), difusión (no_evaluada/restringida/autorizada) e integración (inventariado/preparado/PR/main). La publicación no se infiere del carácter final del documento.

## 8. Piloto XVII y lote ZIP

1. Recibir un único ZIP, conservar original y registrar SHA-256 y manifiesto del lote sin publicación automática.
2. Inventariar Markdown y conciliar con `AGENDA_ACADEMICA_XVII_2026.csv`, `SESIONES_XVII_2026.csv`, `COBERTURA_XVII_MODELO.csv` y las fuentes del expediente.
3. Detectar ausencias, no realización, duplicados, conflictos de IDs, cambios de autoría, integridad, enlaces y derechos de publicación; no inferir realización a partir de agenda.
4. Proponer residencia canónica sin duplicación física y generar registros mínimos de contribuciones, documentos, autores, instituciones, obras, referencias y conceptos solo donde haya evidencia.
5. Clasificar **elegible**, **condicionado** o **pendiente de investigación**, con un manifiesto explícito por archivo.
6. Presentar **una AHE consolidada** con cantidades comprobadas, excepciones sustantivas y alcance preciso. La decisión humana permite operaciones técnicas descritas en el manifiesto, pero no reemplaza consentimientos ni verifica citas automáticamente.
7. Integrar únicamente contenido elegible y autorizado al PR de memorias, reutilizando `#14` si resulta técnicamente viable; mantener los demás originales bajo custodia separada y registrar metadatos publicables.
8. Verificar idempotencia, vínculos, reversibilidad, correspondencia con inventario, derechos y coherencia con el Contrato de Base de Conocimiento Común.
9. Solicitar autorización humana **independiente** para fusionar con `main`.

No fijar cantidad de memorias ni crear PR adicionales para el mismo lote sin necesidad. El trabajo futuro sobre currículos, bibliografía crítica y conceptos podrá enriquecer las relaciones sin reubicar los documentos originales.

## 9. Validación de arquitectura y primera versión funcional

La arquitectura está **aprobada como orientación**; el piloto determinará su validez operativa. Criterios: unicidad canónica, trazabilidad, navegación multidimensional, respeto por autorías y disensos, vínculos verificables, permisos, ausencia de duplicados, reproducibilidad de manifiesto y control de excepciones.

La estabilización funcional requerirá: corpus elegible integrado, índices consistentes, controles básicos ejecutados, problemas residuales documentados, PR revisado y autorización humana de merge. Solo entonces actualizar `README.md` público para expresar identidad, alcance, contenido realmente disponible, límites, estado y forma de navegación. No anunciar integración o versión estabilizada antes de verificarla.

## 10. Referencias del proyecto

- Framework original: `00_CONTROL_MAESTRO/Reglas_Colocacion_Documental/2026-09-22_Regla_Residencia_Semantica_Ciclo_Vida_Documental_v0_1.md` (candidato estructural en la fuente consultada).
- Framework original: `00_CONTROL_MAESTRO/Reglas_Colocacion_Documental/2026-06-05_Protocolo_Manejo_Carpetas_Subcarpetas_Colocacion_Documental_Framework_Generico_V4_1_1_v0_2.md`.
- RIDEG 101: `13_INVESTIGACION_Y_EVIDENCIA/2026-10-05_Contrato_Base_Conocimiento_Comun_V5_v1_0.md` (aprobado y canónico).
- RIDEG 101: `13_INVESTIGACION_Y_EVIDENCIA/RIDEG_101_Acopio/` (inventarios de actas, declaraciones, simposios y memorias).
- RIDEG 101: `18_DOCUMENTACION_ACTIVA/Eventos_Simposios/SIM-XVII_Arequipa_2026/` (expediente operativo del XVII).
- PR de memorias: https://github.com/ricardojuanmorales/rideg-101/pull/14 .

## 11. Gobierno de cambios

Esta versión no autoriza por sí sola publicación de material ajeno, cambios en otras rutas, activación de agentes ni merge. Modificaciones futuras de alcance o residencia requieren decisión humana registrada; la implementación podrá proponer ajustes fundamentados durante el piloto.
