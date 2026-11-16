# Ontología: Fábrica de Software del Instituto Tecnológico Cumbres

## Propósito
Modelar y consultar la trazabilidad operativa entre proyectos de software, sprints, historias de usuario, pruebas automatizadas, defectos, vulnerabilidades en dependencias y despliegues en ambientes del Instituto.

## Versión
`v1.0` — Compatible con OWL 2 DL (sintaxis Turtle).

## Estructura del Repositorio
- `ontologia_v1.ttl`: Esquema formal (14 clases, 21 propiedades).
- `datos_ejemplo.ttl`: Base de conocimiento poblada con 33 individuos.
- `consultas.rq`: Consultas SPARQL correspondientes a las 6 Preguntas de Competencia.
- `especificacion.pdf` / `conceptualizacion.pdf` / `evaluacion.pdf`: Documentación METHONTOLOGY.

## Cómo cargar y validar en Protégé
1. Abrir **Protégé 5.6+**.
2. Seleccionar **File -> Open...** y cargar `datos_ejemplo.ttl` (importará automáticamente `ontologia_v1.ttl` si están en la misma carpeta).
3. En el menú superior, ir a **Reasoner -> HermiT** y hacer clic en **Reasoner -> Start reasoner** (`Ctrl+R`).
4. Abrir la pestaña **SPARQL Query** (o **Snap SPARQL Query** para incluir inferencias) y ejecutar las consultas de `consultas.rq`.