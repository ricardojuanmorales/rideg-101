# Acopio de Memorias históricas RIDEG: catálogo de portal v0.1

**Fecha de revisión:** 2026-11-12. **Estado:** catálogo inicial de referencias públicas, no biblioteca descargada ni certificación de integridad de los documentos enlazados.

## Alcance

La página pública [Memorias](https://www.rideg.org/memorias/) muestra referencias a **siete ediciones:** II, III, IV, V, VI, VII y IX (2010–2017). La falta de otras ediciones **en este índice** no acredita inexistencia de sus memorias o textos; tampoco se debe equiparar los programas enlazados en [Actividades](https://www.rideg.org/actividades/) con memorias definitivas.

Se crea `CATALOGO_MEMORIAS_PORTAL_RIDEG.csv` con un registro **por edición listada**, antes de expandir a un registro por ponencia. Los PDF y recursos individuales **no han sido descargados ni validados exhaustivamente** y por eso no se consignan tamaños, checksums, conteos de archivos o supuestas afiliaciones institucionales.

## Notas de fuentes

- WEB-MEM-INDEX: https://www.rideg.org/memorias/
- WEB-MEM-002: https://www.rideg.org/memorias/ii-simposio/ (ponencias con enlaces de descarga).
- WEB-MEM-003: https://www.rideg.org/memorias/iii-simposio/ (presentación, ponencias y epílogo).
- WEB-MEM-004: https://www.rideg.org/memorias/iv-simposio/ (ponencias por jornadas; disponibilidad parcial en video).
- WEB-MEM-005: https://www.rideg.org/memorias/v-simposio/ (ponencias listadas).
- WEB-MEM-006: https://www.rideg.org/memorias/vi-simposio/ (trabajos listados).
- WEB-MEM-007 y 009: **pendiente identificar y verificar los enlaces de destino desde el índice**.

## Claves de gobierno documental

1. Distinguir **memoria como índice web**, **ponencia listada**, **documento accesible**, **original capturado localmente**, **texto revisado** y **publicación autorizada**.
2. Cada edición se enlaza por numeral con `simposios_2010_2026.csv`. No se alteran sus datos originales desde esta fuente.
3. Cada futura ponencia tendrá ID `PON-{EDICION}-{SEQ}`, título literal, nombres como aparecen en fuente, página que la enumera, URL de archivo, fecha de comprobación y estado. **No inferir afiliaciones de autorías** a partir de instituciones anfitrionas.
4. Un PDF descargado a custodia local se registra con bytes, SHA-256 y nombre exacto; nunca se publica en GitHub sin una revisión de derechos y autorización.
5. Las discrepancias entre fechas, títulos o autorías se registran como observaciones de fuente, no se sobreescriben silenciosamente.
6. Para la cobertura del XVII, utilizar el mismo esquema: **evento → sesión → contribución → fuente → nivel de verificación**, con captura rápida y enriquecimiento posterior.

## Próxima iteración

- Seguir enlaces individuales, contar y catalogar ponencias por edición, verificar recursos no accesibles y distinguir formatos.
- Construir una tabla de temas/ejes y autorías respaldada en los textos reales, no solamente en títulos.
- Conectar ponencias y personas con instituciones **solo cuando figure una afiliación explícita**.
- Comparar con la matriz de sedes y actas para reconstruir una trayectoria académica.
- Después diseñar el protocolo mínimo para entrevistas y registro en tiempo real con pocos campos obligatorios.

**No se afirma que todas las memorias del sitio hayan sido descargadas o preservadas.**
