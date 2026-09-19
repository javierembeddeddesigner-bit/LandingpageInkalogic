# IncaLogic — Landing Page

Contexto de proyecto para Claude Code. Este archivo se carga automáticamente en cada
conversación abierta en esta carpeta, para que todas compartan el mismo entendimiento.

## Qué es esto

Landing page de **IncaLogic**, los primeros PLCs peruanos, desarrollados por
**MMJ Smart Electronics**. Objetivo único de la página: que el visitante **agende una
reunión** (por WhatsApp). Nada de tiendas, catálogos extensos ni formularios largos.

## Sobre el producto (para redactar copy)

- **IncaLogic** = primer PLC diseñado y fabricado en Perú.
- Empresa: **MMJ Smart Electronics** (Perú).
- Ecosistema: **10 controladores núcleo** + **más de 40 módulos de expansión**.
- Diferenciadores clave: ingeniería y soporte local, stock/repuestos en Perú,
  ecosistema escalable (de máquina compacta a planta completa), trato directo con
  el equipo que diseñó el equipo.
- Fundador / contacto: Javier Hernández (javier.embedded.designer@gmail.com).

## Decisiones de diseño (ya tomadas — mantener coherencia)

- **Estilo:** minimalista y profesional. Nada folclórico ni recargado.
- **Acento visual:** cobre/ámbar (`--copper: #b06a3b`) como guiño sutil a la
  metalurgia inca + electrónica industrial, sobre base clara.
- **Tipografía:** Space Grotesk (títulos) + Inter (cuerpo), vía Google Fonts.
- **CTA:** WhatsApp (no formularios). El número y el mensaje se editan en el bloque
  de configuración al final de `index.html` (`WHATSAPP_NUMERO`, `WHATSAPP_MENSAJE`).
- **Sin sección de clientes** por ahora (decisión del cliente).
- Idioma de la página: **español**.

## Estructura del sitio

Un solo archivo autocontenido: `index.html` (sin build, sin dependencias npm).
Secciones: Hero → Cifras (1°/10/40+) → Por qué IncaLogic (3 tarjetas) →
Ecosistema (franja oscura) → CTA final → Footer.

## Convenciones de trabajo

- Mantener `index.html` autocontenido y desplegable tal cual (Netlify/Vercel/hosting).
- Al hacer cambios de UI/diseño, apoyarse en el skill **`frontend-design`**
  (instalado en `.claude/skills/`).
- No introducir un paso de build salvo que se pida explícitamente
  (en este equipo **Node.js/npm no está instalado**).
- Copy en español, tono profesional y directo.

## Estado / pendientes

- [ ] Reemplazar el número de WhatsApp de ejemplo (`51999999999`) por el real.
- [ ] (Opcional) Logo real de MMJ en lugar del ícono SVG del header.
- [ ] (Opcional) Foto real de un controlador IncaLogic en el hero.
- [ ] Desplegar (hosting por definir).
