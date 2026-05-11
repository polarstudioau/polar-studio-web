# Quick Start — Web Delineacion

## Project Structure

```
web-delineacion/
├── src/                    ← Edit these files
│   ├── index.html         (one-page con Hero + 6 servicios + FAQ)
│   ├── about.html         (página About)
│   ├── contact.html       (formulario Netlify)
│   ├── 404.html           (error)
│   ├── polar.css          (sistema de diseño)
│   ├── sitemap.xml
│   └── robots.txt
├── assets/
│   ├── favicon.svg
│   └── polar-logo.jpeg
├── docs/
│   ├── CHANGELOG.md
│   ├── SEO-ROADMAP.md
│   └── CUSTOMIZATION.md
├── netlify.toml
└── README.md
```

---

## Workflow Semanal

### Lunes — Planificar
- Abre `docs/SEO-ROADMAP.md` → ¿Cuál es el foco esta semana?
- Revisa Google Analytics → ¿Qué funciona, qué no?

### Martes-Jueves — Crear
- Edita archivos en `src/`
- Usa `docs/CUSTOMIZATION.md` como guía
- Prueba localmente abriendo `index.html` en el navegador
- Guarda cambios

### Viernes — Deploy
- Arrastra carpeta `src/` a Netlify
- Verifica en staging: `superlative-twilight-e65d1d.netlify.app`
- Actualiza `docs/CHANGELOG.md` con lo que cambiaste
- Cuando DNS esté listo: live en `polarstudio.com.au`

---

## Cómo Pedirme Cambios

Solo dime lo que quieres. Yo sé qué archivo editar.

Ejemplos:
- "Actualiza la descripción del servicio BIM para mencionar AS 1100"
- "Añade un FAQ sobre tiempos de entrega urgentes"
- "Cambia el color principal de azul a teal"
- "Crea una página de blog para artículos"
- "Añade Google Analytics"
- "Crea páginas por ciudad (Sydney, Melbourne, etc.)"

Yo edito → tú subes a Netlify → actualizas CHANGELOG → listo.

---

## Tabla de Referencia Rápida

| Quiero cambiar... | Archivo | Buscar |
|---|---|---|
| Título de servicio | `src/index.html` | `<h2>BIM &...` |
| Descripción servicio | `src/index.html` | `<p class="lead">` |
| Pregunta FAQ | `src/index.html` | `<button class="faq-q">` |
| Respuesta FAQ | `src/index.html` | `<div class="faq-a-inner">` |
| Email | Todos los .html | `polar.estudio.arquitectura@gmail.com` |
| Teléfono | Todos los .html | `+61 0430 141 615` |
| Color principal | `src/polar.css` | `--accent: #2756ff` |
| Tipografía | `src/polar.css` | `--font-display:` |
| Texto About | `src/about.html` | `<div class="mission-row">` |

---

## Deploy a Netlify (3 pasos)

1. Ve a https://app.netlify.com
2. Proyecto: **superlative-twilight-e65d1d**
3. Arrastra carpeta `src/` al área de "Deploys"
4. Espera 1-2 minutos
5. Verifica: `superlative-twilight-e65d1d.netlify.app`

---

## Estado DNS

✅ **Hecho:**
- Web subida a Netlify
- Dominio polarstudio.com.au añadido en Netlify
- A record en GoDaddy → 75.2.60.5

⏳ **Pendiente:**
- CNAME `www` en GoDaddy → `superlative-twilight-e65d1d.netlify.app` (editar el existente, no crear nuevo)
- Propagación DNS (1-24h)
- Activar HTTPS/SSL en Netlify

---

## Tu Plan de la Primera Semana

1. **Lunes:** Lee este archivo + abre los otros docs
2. **Martes:** Resuelve el CNAME en GoDaddy
3. **Miércoles:** Configura Google Analytics + Search Console
4. **Jueves:** Submit sitemap a GSC
5. **Viernes:** Empieza primer artículo de blog

---

## Documentación

| Archivo | Cuándo leerlo |
|---|---|
| `README.md` | Una vez (overview general) |
| `INSTRUCTIONS.md` | Esta semana (quick start) |
| `CHANGELOG.md` | Cada viernes (registrar cambios) |
| `SEO-ROADMAP.md` | Cada lunes (planificar) |
| `CUSTOMIZATION.md` | Antes de cada edición |

---

**Última actualización:** 17 Apr 2025  
**Versión:** 1.0 — Production-ready