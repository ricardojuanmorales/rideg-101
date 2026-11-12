# RIDEG | Documento de Identidad Base

**Versión:** 0.1 · **Fecha de corte del expediente:** 12 de noviembre de 2026 · **Estado:** BORRADOR DOCUMENTAL PARA REVISIÓN HUMANA (no norma ni declaración oficial aprobada).

## 1. Denominación y naturaleza

**Red Internacional de Estudios Generales (RIDEG).** La página oficial «¿Quiénes somos?» la presenta como una comunidad abierta, integrada tanto por instituciones universitarias como por académicos en calidad individual, y como un espacio en evolución. No debe reducirse a un listado cerrado de universidades. **Fuente:** WEB-QUIENES, https://www.rideg.org/quienes-somos-2/.

## 2. Fundación y contexto histórico

La sección oficial «Historia» sitúa su fundación **28–29 de enero de 2010**, en el **Recinto de Río Piedras de la Universidad de Puerto Rico**, durante el **I Simposio Internacional de Estudios Generales**. Indica que seis universidades estuvieron representadas en la Primera Declaración de Río Piedras; **no identifica aquí sus seis nombres**, por lo que no se infieren. **Fuente:** WEB-HISTORIA, https://www.rideg.org/78-2/.

El texto histórico menciona «16 instituciones provenientes de 9 países» tras los encuentros iniciales. Es un **dato correspondiente a la etapa histórica relatada**, no el censo actual; para el inventario inicial de la página «¿Quiénes somos?» se cuentan **24 entradas institucionales** (consulta 2026-11-12), separadas de **3 personas listadas como miembros independientes**.

## 3. Justificación y orientación intelectual

La justificación histórica subraya la necesidad de fortalecer la educación general universitaria frente a desafíos complejos que no pueden atenderse desde saberes fragmentados y descontextualizados. La RIDEG promueve formación integral, integración de saberes, reflexión crítica, colaboración y renovación de los Estudios Generales. Esta es una **síntesis editorial** de la sección «Historia», no una nueva declaración de principios aprobada. **Fuente:** WEB-HISTORIA.

## 4. Objetivos publicados en el portal histórico

El portal enumera seis campos de acción que se registran aquí en forma sintética:

1. Auspicio de simposios internacionales dedicados a la educación general y a los Estudios Generales.
2. Seminarios y líneas de investigación para profundizar problemas académicos.
3. Diálogo e intercambio entre instituciones, incluyendo profesorado, estudiantado, talleres, encuentros y proyectos; uso de tecnologías y redes.
4. Propuestas conjuntas para enriquecer experiencias estudiantiles y la formación continua del profesorado.
5. Investigación y documentación histórica sobre los Estudios Generales en el continente.
6. Publicación y difusión de libros y otros materiales pertinentes.

**Fuente:** WEB-HISTORIA. El portal relata además aspiraciones históricas de formación de posgrado itinerante y colaboración regional. No se declara que estas aspiraciones hayan sido ejecutadas.

## 5. Condiciones de vinculación reportadas

La historia del portal señala la expresión de interés, el compromiso de colaboración según las posibilidades de cada institución, la designación de un contacto y la difusión de proyectos/actividades. **No se interpreta esta descripción como un procedimiento formal vigente o reglamento aprobado sin respaldo documental adicional.** Fuente: WEB-HISTORIA.

## 6. Composición institucional y personal

El directorio «¿Quiénes somos?» lista **24 instituciones** y, en apartado distinto, **3 miembros independientes**. El registro maestro `INSTITUCIONES_RIDEG.csv` captura los 24 nombres junto a sus países/territorios y unidades académicas reportadas; añade otras tres entidades mencionadas en la historia de sedes, **sin atribuirles membresía formal**. El portal incluye contactos personales, pero esta versión del inventario prioriza registros institucionales y **no reproduce correos personales**.

**Fecha de consulta** no equivale a fecha de incorporación, ratificación o vigencia de membresía. Necesitamos cotejar actas, declaraciones, correspondencia institucional y confirmación de representantes para un inventario de afiliaciones formalmente validado.

## 7. Sedes y relación con los simposios

La matriz `INSTITUCIONES_SIMPOSIOS.csv` documenta **17 relaciones principales entre edición y sede/organizadora** desde 2010 hasta la XVII edición anunciada para 2026. La XII edición se realizó virtualmente según la matriz histórica: en ese caso se consigna **organizadora**, no sede física del evento. Las instituciones repetidas mantienen el mismo identificador estable. Esta matriz **no demuestra que todas las instituciones del directorio hayan sido sede**, ni pretende registrar todas las presentaciones de participantes.

## 8. Gobernanza del inventario

- Diferenciar **listada en directorio**, **miembro independiente**, **anfitriona/organizadora**, **colaboradora** y **participante**.
- Para cada vínculo registrar fuente, fecha de observación, período de vigencia (cuando conste), condición de verificación y decisión de revisión.
- Conservar grafías originales e indicar nombres normalizados solo con evidencia (por ejemplo Universidad Nacional Federico Villarreal).
- **No borrar registros históricos**: anotar ceses, cambios de denominación y relaciones previas mediante historial/versiones.
- Actualizar la matriz de instituciones y la de relaciones mediante nuevos commits y PR; no equiparar automáticamente alojamiento de simposio con afiliación formal.
- Evitar publicar datos de contacto de personas sin necesidad documental y autorización apropiada.

## 9. Pendientes de corroboración

- Vigencia de afiliaciones y representación actual de las 24 instituciones del directorio.
- Identificación nominal y documental de las seis universidades firmantes originales.
- Confirmación de denominaciones históricas de las sedes VIII y XI, y categorías de colaboración de cada edición.
- Identificación de instituciones participantes en las ponencias del XVII, en registro separado del de las sedes (programa no acredita asistencia efectiva).
- Resolución formal de discrepancias históricas de fechas del I y XII.

## Fuentes

- **WEB-QUIENES:** https://www.rideg.org/quienes-somos-2/ (consulta 2026-11-12).
- **WEB-HISTORIA:** https://www.rideg.org/78-2/ (consulta 2026-11-12; texto histórico posiblemente anterior).
- **DOC-001:** tabla de 17 simposios, ya registrada en acopio RIDEG 101.
- **DOC-002:** programa de ponencias del XVII Simposio, utilizado para situar la edición 2026.
