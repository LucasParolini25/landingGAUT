# Pendientes — Landing GAUT

Última actualización: 30/10/2026 · Sitio: https://www.gaut.com.ar/ (Vercel, publica desde `main`)
El estado de las tareas de marketing vive en Trello (MKT-7: revisión de la landing). Este archivo junta lo puntual de la landing.

## Necesitan algo de Lucas
- [ ] **Imagen para la vista previa al compartir** — 1200 × 630 px, PNG o JPG, < 1 MB.
  Fondo `#0B1120`, logo nuevo (sin texto abajo) arriba a la izquierda, frase "¿TENÉS UNA FLOTA Y LA ALQUILÁS A CHOFERES DE APPS?"
  ("CHOFERES DE APPS" en `#F5B800`, fuente Barlow Condensed), captura del panel a la derecha, 60 px de margen.
  Guardar como `uploads/og-image.png` → después hay que cambiar `og:image` y `twitter:image` en `index.html`
  (hoy apuntan a `uploads/dashboard-adm.png`).
- [ ] **Prueba social (MKT-7)** — franja "Ya lo usan flotas en Tucumán y Salta" + versión corta del caso (OFE-5 ya está aprobada). Falta que Lucas apruebe el texto.
- [ ] **Tareas de SEO de Lucas (MKT-7)** — {{completar}}.
- [ ] **Precio o planes** — aunque sea "desde $X/mes" o "según cantidad de autos". Los precios base están definidos (OFE-1); falta decidir si se muestran en la landing.
- [ ] **Testimonios** — una o dos frases de clientes o de la prueba piloto, con nombre y cantidad de autos.
- [ ] **Google Business Profile** (business.google.com) — categoría "Empresa de software", web `https://www.gaut.com.ar/`.
- [ ] **Links en redes** — poner `https://www.gaut.com.ar/` en Instagram, LinkedIn y WhatsApp Business.

## Revisar en unos días
- [ ] **Google**: buscar `site:gaut.com.ar` y confirmar que aparezcan el título y la descripción nuevos y el logo.
      Si no, volver a tocar "Solicitar indexación" en Search Console.
- [ ] **Search Console → Sitemaps**: `https://www.gaut.com.ar/sitemap.xml` con estado "Correcto".
- [ ] **Vercel → Analytics**: que se registren visitas.
- [ ] **Clarity** (proyecto `yndomxbpve`): revisar grabaciones y el evento `whatsapp_click`
      (filtro por la etiqueta `whatsapp_origen` para ver qué botón usan más).

## Puedo hacerlo sin datos tuyos
- [ ] Aviso o página corta de privacidad (por Clarity y Analytics).
- [ ] Sacar la dependencia de React desde unpkg / `support.js` y dejar la página en HTML simple (más rápida y sin depender de servicios externos).
- [ ] Más adelante: notas para SEO (ej. "Cómo calcular el excedente de km", "Cuánto deja un auto alquilado a choferes de apps").

## Hecho el 26/10/2026 (marca nueva)
- "Gestión de Alquiler Uber y Taxi" → "Gestión de flotas" (footer y datos estructurados); "y taxi" en la meta description.
- Logo nuevo sin texto en header y footer (`alt="GAUT"`), favicon 32 px y apple-touch-icon 180 px.
- Preguntas frecuentes: "desde 10 autos en adelante, con una o varias sucursales".
- Links a Facebook e Instagram (`gautflotas`) en el footer y en `sameAs`.

## Hecho el 23–24/09/2026
- Hero con textos nuevos y sección de Preguntas frecuentes.
- Scroll en mobile sobre las imágenes arreglado.
- SEO: title, description, Open Graph, datos estructurados, alt en imágenes, sitemap.xml, robots.txt, favicon 192 px.
- Search Console verificado por DNS en DonWeb (no borrar el registro TXT).
- Imágenes en WebP (~790 KB → ~91 KB), contacto clickeable, botones "Quiero una demo" unificados.
- Menú desplegable en mobile, footer sin nota de tesis.
- Vercel Analytics y Microsoft Clarity con registro de clics a WhatsApp.
