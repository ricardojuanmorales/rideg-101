# Flujo bidireccional de trabajo: RIDEG 101 ↔ GitHub

## Propósito
El repositorio `ricardojuanmorales/rideg-101` es el registro versionado de los documentos, fuentes y productos aprobados de la Memoria Histórica de la Red Internacional de Estudios Generales. ChatGPT se utiliza como espacio de análisis, redacción y apoyo, sin reemplazar el historial verificable de GitHub.

## Principios
- `main` es la rama estable; no se escribirá en ella directamente mediante este flujo.
- Cada cambio comienza en una rama de trabajo creada desde la versión más reciente de `main`.
- Toda integración a `main` requiere un pull request (PR), revisión de diferencias y aprobación humana explícita.
- No fusionar PR automáticamente por el mero hecho de haberlos creado o revisado.
- Documentos canónicos, fuentes históricas y decisiones institucionales requieren revisión especialmente cuidadosa: mantener procedencia, citas, fecha, autoría y rastreabilidad.
- No subir datos personales, credenciales ni materiales con permisos inciertos.

## Ciclo operativo
1. **Leer / sincronizar:** consultar `main`, su README, documentos existentes, PR abiertos y cambios recientes antes de iniciar una tarea; identificar la versión fuente.
2. **Definir:** registrar objetivo, alcance, documentos afectados y criterios de aceptación.
3. **Crear rama:** usar `docs/<tema>`, `feat/<tema>`, `fix/<tema>` o `chore/<tema>` según el cambio.
4. **Producir:** preparar análisis y contenido en ChatGPT; contrastar con las fuentes del repositorio antes de publicar.
5. **Proponer:** registrar commits descriptivos en la rama y abrir PR contra `main`, preferiblemente como borrador mientras está en elaboración.
6. **Revisar:** examinar diferencias, referencias, integridad documental y conflictos. Incorporar correcciones en la misma rama.
7. **Aprobar e integrar:** solicitar decisión humana; fusionar solo tras la aprobación explícita correspondiente y las comprobaciones configuradas.
8. **Cerrar el ciclo:** releer `main`, resumir el cambio integrado y registrar pendientes o enlaces a PR, evitando asumir que un PR abierto ya está integrado.

## Convenciones mínimas
- Commits: `docs: ...`, `feat: ...`, `fix: ...`, `chore: ...`.
- PR: indicar contexto, cambios, fuentes, validaciones, riesgos, asuntos pendientes y decisión requerida.
- Evitar sobrescribir silenciosamente archivos: revisar contenido y SHA vigente antes de actualizarlos.
- Las discusiones en ChatGPT que no estén incorporadas a commits/PR no forman parte por sí solas del repositorio.
- Si la conexión o permisos de GitHub fallan, detener escrituras e informar, sin dar por guardados los cambios.

## Protección recomendada en GitHub
En **Settings → Rules → Rulesets** (o protección de ramas), configurar una regla para `main` que requiera PR antes de fusionar. Si existe un revisor independiente, exigir al menos una aprobación; también considerar resolución de conversaciones y bloqueo de force-push/eliminación. Un repositorio con un solo mantenedor puede necesitar un esquema de revisión propio y una configuración distinta para no bloquear sus aportaciones. Estas reglas no se activan por la existencia de este documento y deben verificarse en GitHub.

## Límite de la integración
La conexión permite operaciones bajo autorización de la cuenta enlazada; no garantiza sincronización automática ni continua entre sesiones. Cada operación importante debe releer el estado remoto. Este protocolo no establece una tarea de fondo ni una integración automática.
