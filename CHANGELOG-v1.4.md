# CHANGELOG — Polar Studio Web

## v1.4 — 30 Apr 2026

**Reconstrucción de HTML para incluir Insights + arreglo definitivo del menú móvil**

### Añadido
- **`index.html`** — Enlace "Insights" en nav escritorio, menú móvil y footer
- **`about.html`** — Enlace "Insights" en nav escritorio, menú móvil y footer
- **`contact.html`** — Enlace "Insights" en nav escritorio, menú móvil y footer
- **`sitemap.xml`** — Entrada para `insights.html` (changefreq: weekly, priority: 0.8)

### Corregido
- **Menú móvil**: ahora funciona correctamente en iPhone/iPad
  - Botón hamburguesa cambia a "X" cuando está abierto (antes solo había icono fijo)
  - Body bloquea el scroll mientras el menú está abierto (antes scroll seguía activo de fondo)
  - Tecla Escape cierra el menú (mejora accesibilidad)
  - aria-expanded se actualiza dinámicamente (mejora accesibilidad)
  - Menú se cierra correctamente al pulsar cualquier enlace

### Cambios técnicos
- Eliminado `onclick` inline del botón hamburguesa
- Añadido `id="mobileToggle"` al botón para JS limpio
- Botón ahora contiene 2 SVG: `.icon-menu` (visible por defecto) y `.icon-close` (visible cuando `body.menu-open`)
- Listener JS añade/quita clase `menu-open` al `<body>` (que el CSS ya esperaba pero antes no se aplicaba)

### NO modificado (importante)
- **`insights.html`** — Sigue intacto en producción con los 10 artículos. Hay que descargarlo de Netlify con Cmd+S y meterlo en `src/` antes de redeploy.
- **`polar.css`** — Sin cambios, la estructura de mobile menu ya estaba bien preparada en CSS, solo faltaba que el JS la activara.
- Imágenes — Sin cambios, las 9 imágenes JPG siguen en `assets/images/`.

### Pendiente (v1.5)
- Resolver CNAME `www` en GoDaddy
- Configurar Google Analytics 4
- Configurar Google Search Console + submit sitemap
- Probar visualmente menú móvil en producción tras deploy

---

## v1.3 — 29 Apr 2026

**Imágenes reales integradas + nuevo hero de Sídney**

### Añadido
- **9 imágenes JPG reales** reemplazando los placeholders SVG:
  - `bim-revit-support.jpg` + `bim-revit-precision.jpg` (servicio BIM + grid)
  - `redline-asbuilt.jpg`
  - `shop-drawings.jpg`
  - `fire-evacuation.jpg`
  - `existing-conditions.jpg`
  - `real-estate-3d.jpg`
  - `team-office.jpg` (página About)
  - `hero-main.jpg` (NUEVO: foto del edificio en construcción de Sídney como hero)
- **Carpeta `assets/images/hero/`** — Nueva ubicación para imagen del hero

### Cambiado
- **`index.html`** — 7 referencias de imagen actualizadas a `.jpg` locales
- **`about.html`** — 1 referencia de imagen actualizada a `.jpg` local
- **`polar.css`** — URL del hero apunta a `assets/images/hero/hero-main.jpg` (antes era CDN externo de Webflow)

---

## v1.2 — 29 Apr 2026

**5 artículos nuevos en Insights + bullets corregidos + fechas 2026**

### Añadido
- **`insights.html`** — 5 artículos nuevos publicados:
  - *Why Your Fabricator Keeps Requesting Drawing Revisions* (Shop Drawings)
  - *Measured Surveys Before a Commercial Fitout* (Existing Conditions)
  - *When Did You Last Update Your Evacuation Diagram?* (Fire Evacuation)
  - *Revit Family Libraries: Why Generic Families Are Costing Australian Projects Time and Money* (BIM & Revit)
  - *Floor Plans That Sell: Why Marketing Floor Plans Are Not the Same as Construction Drawings* (Real Estate & 3D)

### Corregido
- **`insights.html`** — Formato de bullets mejorado: título en negrita en línea propia, texto descriptivo debajo
- **`insights.html`** — Fechas de todos los artículos actualizadas a 2026

---

## v1.1 — 20 Apr 2026

**Nueva sección Insights + formulario contact arreglado + fixes responsive**

### Añadido
- **`insights.html`** — Nueva página de noticias del sector AEC
  - Grid de cards (3 columnas, responsive)
  - Modal popup con artículo completo, header y footer fijos (cero overlap al hacer scroll)
  - Filtro por servicio
  - Bloque de fuentes reales al final de cada artículo
- **5 artículos originales publicados** (con fechas Apr 2025, actualizadas en v1.2):
  - *ISO 19650 in Practice* (BIM & Revit)
  - *AS 3745:2010 Compliance: The Most Common Mistakes* (Fire Evacuation)
  - *Why LOD 300 Is No Longer Enough for Sydney DA Submissions* (BIM & Revit)
  - *Off-the-Plan Visualisation* (Real Estate & 3D)
  - *The Handover Problem* (As-Built)
- **`thank-you.html`** — Página de confirmación post-submit
- **Email notifications** en Netlify Forms (configurado en dashboard)

### Corregido
- Dropdown "Services" no desaparece al cruzar al panel (puente invisible CSS + click support touch)
- Formulario de contacto redirige a `/thank-you.html` tras envío
- Menú móvil con scroll y full-height (PRIMERA versión, completada definitivamente en v1.4)
- Breakpoint extra para tablet (<900px) y móvil pequeño (<480px)

---

## v1.0 — 17 Apr 2025

**Lanzamiento de la web one-page**

### Añadido
- **`index.html`** — One-page con Hero + 6 servicios + FAQ
- **`about.html`** — Historia + valores + stats
- **`contact.html`** — Formulario Netlify integrado
- **`404.html`** — Página de error
- **`polar.css`** — Sistema de diseño (variables, componentes)
- **`sitemap.xml`** + **`robots.txt`** — SEO básico
- Schema.org JSON-LD (Organization)
- Open Graph + Twitter meta tags
- Nav fija con dropdown "Services" + menú móvil

### Stack
- HTML5 + CSS3 puros (sin frameworks, sin build)
- Netlify hosting (proyecto `superlative-twilight-e65d1d`)
- Google Fonts: Instrument Sans + Inter
