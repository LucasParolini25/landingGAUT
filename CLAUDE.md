# CLAUDE.md — Landing GAUT (área Marketing)
> Reglas para trabajar en la landing pública https://www.gaut.com.ar/. Es parte del área **MKT** (ver `GAUT/CLAUDE.md`, tabla de Áreas).
> Las reglas generales (inicio de sesión, Engram, Trello, qué necesita a Lucas) están en `GAUT/CLAUDE.md`.

---

## Qué es

- Sitio estático de una sola página: `index.html` (HTML + CSS inline), imágenes en `uploads/`, `robots.txt` y `sitemap.xml`.
- `support.js` e `image-slot.js` son runtime generado por la herramienta de diseño original: **no editarlos a mano**.
- Medición: Vercel Analytics y Microsoft Clarity (proyecto `yndomxbpve`, evento `whatsapp_click` con la etiqueta `whatsapp_origen`).
- Pendientes de la landing: `PENDIENTES.md`. La revisión grande (marca nueva, SEO, prueba social) es la tarea **MKT-7**.

---

## Deploy — lo decide Lucas

- **Vercel publica automáticamente cada push a `main`** en www.gaut.com.ar. Un push a `main` es una publicación: solo Lucas lo hace.
- Flujo como en gaut-webapp: rama (`feat/<tema>` o `fix/<tema>`, desde `develop`) → `develop` → `main`. Claude trabaja en la rama, commitea ahí y le avisa a Lucas qué revisar.
- Lucas pasa la rama a `develop` y la sube: Vercel arma una vista previa (Preview) para revisar antes de publicar. Después pasa `develop` a `main`.
- Nunca push ni merge a `develop` o `main`, force push, rebase ni borrar ramas.
- El dominio está en DonWeb. **No tocar** el registro TXT de verificación de Search Console.

---

## Reglas de contenido

- Textos en español rioplatense con voseo, tono profesional y directo (voz de marca en `gaut-negocio/contexto/voz.md`).
- Colores, tipografía y logo: solo los tokens de `GAUT/docs/DISENO.md`.
- No inventar precios, clientes, testimonios ni números. Si falta un dato, dejar `{{dato}}` y avisar.
- Imágenes nuevas en WebP dentro de `uploads/`; las capturas del sistema salen de `GAUT/capturas-GAUT/`.
- Al cambiar título, descripción o imagen de vista previa, revisar también las etiquetas `og:*`, `twitter:*` y el JSON-LD de `index.html`.

---

## Git

- Commits con Conventional Commits en español (`feat: ...`, `fix: ...`, `chore: ...`), staging de archivos puntuales (nunca `git add .` ni `-A`).
- `.atl/` está ignorado (lo genera el registro de skills).

---

## Cómo probar

Abrir `index.html` en el navegador (no hay build). Revisar en ancho de celular: la mayoría de las visitas entra desde el teléfono.
