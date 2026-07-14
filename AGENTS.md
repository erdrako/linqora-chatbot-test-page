

<!-- LINQORA_SHARED_AGENT_GUIDELINES:BEGIN -->
# Guias Compartidas Para Agentes Linqora

Fecha de ultima revision: 2026-07-13.

Estas reglas pueden sincronizarse dentro de `AGENTS.md` usando marcadores
controlados. Las reglas locales de cada repo deben permanecer fuera del bloque
generado.

## Contexto Inicial

Antes de planificar o implementar cambios:

1. Revisar `docs/PROJECT_STATUS.md` o el mirror local equivalente.
2. Revisar `README.md`.
3. Revisar los documentos especificos del area a tocar.
4. Si el cambio cruza repos o afecta roadmap, riesgos, deploy, arquitectura o
   pendientes, revisar `linqora-project/docs/PROJECT_STATUS.md`.

## Documentacion Y Estado

- Usar fechas absolutas `YYYY-MM-DD`.
- Documentar decisiones relevantes antes de implementar cuando el cambio afecte
  arquitectura, operacion, datos, deploy o estado de producto.
- Actualizar `docs/PROJECT_STATUS.md` cuando cambien estado, pendientes,
  riesgos, deploys, fuentes de verdad o proximos pasos.
- Al actualizar archivos generados de gobernanza, mantener el cambio enfocado y
  evitar churn de formato no relacionado.
- Los cambios generados de `AGENTS.md` deben seguir siendo revisables y no
  incluir cambios runtime.
- Cuando algo quede "a monitorear", "congelado", "para mas adelante" o
  "pendiente de analizar", registrar fecha absoluta y razon breve.

## Seguridad

- No versionar secretos.
- No leer ni exponer `secrets.md`, `api-keys/`, `.env` ni `.dev.vars` salvo
  pedido explicito para una tarea operativa concreta.
- No copiar tokens al chat ni a documentacion.
- Documentar problemas operativos repetibles sin incluir valores sensibles.

## GitHub Y Operacion

- Mantener issues y PRs tecnicos en el repo responsable.
- Usar `linqora-project` para contexto global, gobernanza, roadmap, riesgos y
  coordinacion cross-repo.
- Usar el GitHub Project como tablero operativo y mantener `Workflow status`
  como estado primario.
- No cerrar items que dependen de actividad real o decision externa; dejarlos
  clasificados como `Ready`, `Blocked` o `Parked` segun corresponda.
<!-- LINQORA_SHARED_AGENT_GUIDELINES:END -->

<!-- LINQORA_REPOSITORY_AGENT_GUIDELINES:BEGIN -->
# Reglas Locales De linqora-chatbot-test-page

Fecha: 2026-07-14.

`linqora-chatbot-test-page` es una pagina estatica minima para probar el widget
publico.

## Reglas

- No convertirla en una aplicacion compleja.
- Mantener bot ID y widget como configuracion explicita.
- Validar que siga cargando el asset productivo
  `https://chat.linqorait.com/widget.js`.
- No agregar secretos ni build innecesario.
- Repo `main`-only.

## Politica De Ramas

La politica general de ramas, promociones y ambientes de Linqora se mantiene en:

https://github.com/erdrako/linqora-project/blob/main/docs/governance/branch-promotion-policy.md
<!-- LINQORA_REPOSITORY_AGENT_GUIDELINES:END -->
