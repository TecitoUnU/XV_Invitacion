# Invitación digital · Mis XV años

Sitio estático (HTML + CSS + JS), listo para GitHub Pages.

## 1. Qué archivos editar

| Archivo | Qué contiene |
|---|---|
| `index.html` | Todo el texto: nombre, fecha, lugar, dirección, links de regalos. Busca los comentarios `<!-- EDITABLE -->` |
| `script.js` | La fecha exacta del countdown y tu número de WhatsApp |
| `style.css` | Los colores (arriba del archivo, sección `:root`), por si quieres ajustar tonos |

### Datos que YA debes cambiar antes de publicar:

1. **Nombre** — en `index.html`, busca `Sofía` (aparece en el hero, la letra del monograma "S" y el footer).
2. **Fecha y hora** — en `script.js`, línea:
   ```js
   const EVENT_DATE = new Date('2026-11-14T19:00:00-06:00');
   ```
   Cambia año-mes-día y hora. El `-06:00` es la zona horaria de Guatemala, no lo quites.
3. **WhatsApp** — en `script.js`:
   ```js
   const WHATSAPP_NUMBER = '50212345678'; // tu número con código de país, sin +
   const WHATSAPP_MESSAGE = '...';
   ```
4. **Lugar, hora y dirección de la misa y la recepción** — en `index.html`, dentro de `<section class="evento">`.
5. **Links de "Ver ubicación"** — reemplaza `href="https://maps.google.com"` por el link real de Google Maps de cada lugar (ábrelo en Maps, botón "Compartir" → copiar link).
6. **Mesa de regalos** — reemplaza los `href="#"` de las tarjetas por tus links reales.
7. **Galería de fotos** — en `index.html`, sección `<section class="galeria">`, reemplaza cada:
   ```html
   <div class="galeria__item ph">1</div>
   ```
   por:
   ```html
   <img class="galeria__item" src="assets/foto1.jpg" alt="">
   ```
   Sube tus fotos a una carpeta `assets/` junto a `index.html`.

## 2. Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (puede ser público o privado si tienes plan que lo permita; para Pages gratis normalmente debe ser público).
2. Sube estos 3 archivos (`index.html`, `style.css`, `script.js`) y tu carpeta `assets/` si agregaste fotos, a la raíz del repositorio.
3. Ve a **Settings → Pages**.
4. En "Source" elige la rama `main` y la carpeta `/ (root)`. Guarda.
5. Espera 1-2 minutos. Tu link quedará como:
   `https://tu-usuario.github.io/nombre-del-repositorio/`
6. Ese es el link que compartes por WhatsApp para la invitación.

## 3. Probarlo antes de compartir

Abre `index.html` haciendo doble clic para verlo en tu navegador antes de subirlo, así confirmas que los datos quedaron bien.
