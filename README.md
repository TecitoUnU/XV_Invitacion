# Invitación digital · Mis XV años

Sitio estático (HTML + CSS + JS), listo para GitHub Pages.

## 1. Qué archivos editar

| Archivo | Qué contiene |
|---|---|
| `index.html` | Todo el texto: nombre, fecha, lugar, dirección, links de regalos. Busca los comentarios `<!-- EDITABLE -->` |
| `script.js` | La fecha exacta del countdown y tu número de WhatsApp |
| `style.css` | Los colores (arriba del archivo, sección `:root`), por si quieres ajustar tonos |

### Ya están cargados estos datos:

- Nombre: **Valeria** (hero, monograma "V" y footer)
- Fecha: **26 de septiembre de 2026**, countdown apuntando a las 4:00 PM
- Padres: **Bétzi Marroquín & David Ruano**
- Misa: 4:00 PM, Iglesia Nuestra Señora del Carmen
- Recepción: 5:30 PM, Salón Centro de Convenciones Las Torrelleanas
- Itinerario: Misa 4:00 PM · Recepción 5:30 PM · Cena 6:30 PM · Baile 7:30 PM
- Código de vestimenta: evitar rosado, celeste y plateado
- Pases: 2 lugares reservados
- Sugerencia de regalo: en efectivo, con sobre el día del evento

### Lo único que falta que agregues tú:

1. **WhatsApp** — en `script.js`:
   ```js
   const WHATSAPP_NUMBER = '50212345678'; // tu número con código de país, sin +
   const WHATSAPP_MESSAGE = '...';
   ```
2. **Links de "Ver ubicación"** — en `index.html`, reemplaza cada `href="https://maps.google.com"` por el link real de Google Maps de la iglesia y del salón (ábrelo en Maps, botón "Compartir" → copiar link).
3. **Galería de fotos** — en `index.html`, sección `<section class="galeria">`, reemplaza cada:
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
