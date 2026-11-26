# KLMoto - Instrucciones persistentes

Antes de trabajar, consulta:

- docs/PRODUCT.md
- docs/ARCHITECTURE.md
- docs/ROADMAP.md
- docs/context/project-context.md
- docs/context/open-questions.md

## Comando de resumen

Cuando el usuario escriba exactamente `Iniciar resumen`, responde primero:

> Modo resumen iniciado.

Luego ejecuta estas acciones:

1. Resume la conversación disponible en la sesión actual.
2. Actualiza `docs/sessions/AAAA-MM-DD.md` con fecha real:
    - hechos confirmados;
    - decisiones confirmadas;
    - pendientes;
    - riesgos o contradicciones.
3. Actualiza `docs/context/project-context.md` únicamente con información confirmada.
4. Actualiza `docs/context/open-questions.md` con preguntas pendientes.
5. No reproduzcas el historial completo.
6. No registrés una decisión nueva sin confirmación explícita.
7. Presenta un resumen de los cambios antes de modificarlos.