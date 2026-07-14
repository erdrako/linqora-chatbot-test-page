# Linqora Chatbot Test Page

Landing estatica para probar una implementacion puntual del widget publico de
Linqora IT.

## Widget

```html
<script src="https://chat.linqorait.com/widget.js" data-bot-id="bot_ded58b53-30f3-452f-85e9-f070039fcfbe"></script>
```

## Cloudflare Pages

- Build command: ninguno.
- Build output directory: `/`.
- Production branch: `main`.

La pagina no usa Vite ni variables de entorno. Cloudflare Pages debe servir los
archivos estaticos directamente desde el repo.

## Gobernanza

Las guias compartidas para agentes se mantienen en `AGENTS.md`. La fuente
central es `linqora-project`, y el workflow `Validate AGENTS` detecta drift
cuando el repo tiene configurado `LINQORA_GOVERNANCE_TOKEN`.
