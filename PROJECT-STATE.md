# PROJECT STATE — Polar Studio Website

**Última actualización:** 30 Abril 2026 18:45 AEST  
**Actualizado por:** Usuario + Claude (conversación actual)

---

## 🎯 ESTADO ACTUAL DEL SITIO

### Páginas existentes (TODAS creadas y funcionando)
- ✅ `index.html` — Homepage con hero + 6 servicios + FAQ
- ✅ `about.html` — Historia + valores + stats
- ✅ `contact.html` — Formulario Netlify
- ✅ `insights.html` — Blog con 10 artículos completos
- ✅ `thank-you.html` — Página de confirmación post-formulario
- ✅ `404.html` — Página de error

### Archivos técnicos
- ✅ `polar.css` — Sistema de diseño completo
- ✅ `sitemap.xml` — Actualizado con lastmod 29/04/2026
- ✅ `robots.txt` — Mejorado con permisos específicos
- ✅ `google16ac3a4bb2156bc7.html` — Verificación Search Console
- ✅ `netlify.toml` — Configuración deploy

### Assets
- ✅ `polarlogo.jpeg` — Logo principal
- ✅ `favicon.svg` — Favicon
- ✅ **8 imágenes nuevas** — subidas en conversación "delineacion" (hero + about + 6 servicios)

---

## 🔧 INTEGRACIONES ACTIVAS

### Google
- ✅ **Google Analytics:** `G-6DPJ8CY549` — instalado en los 4 HTML principales
- ✅ **Search Console:** Verificado + sitemap enviado
- ✅ **Business Profile:** Creado, verificación por correo pendiente

### SEO
- ✅ Schema.org: ProfessionalService + FAQPage + AboutPage + ContactPage
- ✅ Open Graph completo en todas las páginas
- ✅ Geo-targeting: `AU-NSW` + Sydney
- ✅ Meta titles optimizados (< 60 chars)
- ✅ Meta descriptions optimizadas (< 160 chars)

### Automatización
- ✅ Formulario contact → Netlify Forms → Google Apps Script → Sheet + email

---

## 🚨 PROBLEMAS CONOCIDOS

### BAJA PRIORIDAD
1. **Menú móvil/hamburguesa NO funciona** — el dropdown no abre en viewport pequeño (tablet/móvil)
   - Reportado: 20 Abril 2026
   - Estado: Pendiente arreglo (NO es prioridad actual)
   - Archivos afectados: `index.html`, `about.html`, `contact.html`, `insights.html`

### COMPLETADO
2. ✅ ~~Imágenes externas CDN~~ — Resuelto, imágenes propias subidas
3. **Logo Open Graph** — actual es cuadrado, conviene 1200x630px para redes sociales (nice to have)

---

## 📝 CONTENIDO

### Insights (10 artículos publicados)
1. BIM LOD 500 en Australia
2. AS 1100 vs ISO 19650
3. Fire Evacuation Diagrams AS 3745
4. Shop Drawings fabricación acero
5. Redline Cleanup proceso
6. As-Built vs As-Designed
7. Revit Family Creation mejores prácticas
8. Existing Conditions survey workflow
9. BIM Clash Detection coordinación MEP
10. Floor Plans inmobiliarios vs construcción

### FAQs (5 preguntas)
- Turnaround times
- Standards compliance
- File formats
- Urgent deadlines
- Project requirements

---

## 🎨 DISEÑO

### Paleta
- `--bg: #f4f4f2` (fondo crema)
- `--bg-dark: #0a0a0a` (hero, footer)
- `--ink: #111111` (texto)
- `--accent: #2756ff` (azul)

### Tipografía
- Display: Instrument Sans
- Body: Inter

### Identidad visual pendiente
- ⏳ 8 imágenes nuevas estilo: renders 3D arquitectónicos limpios, tonos cálidos (beige/madera)
- Usuario generando en Adobe Firefly

---

## 🔄 DEPLOY

### Hosting
- Plataforma: Netlify
- Proyecto: `superlative-twilight-e65d1d`
- URL staging: `superlative-twilight-e65d1d.netlify.app`
- Dominio: `polarstudio.com.au`

### DNS (GoDaddy)
- ✅ A record → 75.2.60.5
- ⏳ CNAME www pendiente configuración

---

## 📊 ROADMAP SEO (Próximos pasos)

1. ✅ ~~Google Analytics + Search Console + Business Profile~~
2. ✅ ~~Schema markup avanzado~~
3. ✅ ~~Meta tags optimizados~~
4. ✅ ~~Imágenes originales~~
5. ⬜ Crear artículo técnico mensual (calendario pendiente)
6. ⬜ Logo Open Graph 1200x630px
7. ⬜ Backlinks (directorios AEC Australia)
8. ⬜ Arreglar menú móvil (baja prioridad)

---

## 💬 NOTAS CONVERSACIÓN

### Decisiones importantes
- **NO crear páginas por ciudad** — una sola web para toda Australia
- **Idioma web:** Inglés australiano (realise, not realize)
- **Idioma conversación:** Castellano de España (vosotros, vale, ordenador, móvil)
- **Outreach comercial:** se gestiona en OTRO proyecto ("Polar Studio — Normativa & Outreach")

### Preferencias usuario
- Editar directo sin pedir permiso línea por línea
- Recordar anotar en CHANGELOG.md al terminar (pero no hacerlo automático)
- Si cambio afecta varios archivos, hacerlos todos sin pedirlo
- No improvisar código — pedir archivos si no los tengo
- No usar emojis en código, sí en conversación
- Ser proactivo con sugerencias al final con "💡 Sugerencia:"

---

## 🔍 PARA CLAUDE: CÓMO USAR ESTE ARCHIVO

**Al empezar cualquier conversación:**
1. Lee este archivo PRIMERO
2. Busca en `conversation_search` si hay contexto adicional sobre el tema
3. Verifica archivos en `/mnt/project/` para confirmar estado real
4. Si el usuario pide algo que ya existe (ej: insights), avisa y pregunta si quiere actualizar

**Al terminar cualquier sesión:**
1. Actualiza este archivo con cambios realizados
2. Mueve tareas de "⏳ PENDIENTE" a "✅ HECHO"
3. Añade nuevos problemas conocidos si aparecen
4. Actualiza fecha de "Última actualización"

---

**FIN PROJECT-STATE.md**
