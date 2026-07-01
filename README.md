# Gordos' Burgers — Link in bio

Página de una sola carilla (estilo Linktree) con estética *glassmorphism*, hecha en **un solo archivo**: [`index.html`](index.html). Sin dependencias, sin build.

## ✏️ Cómo personalizarla (1 minuto)

Abrí `index.html` y buscá el bloque **`CONFIG`** (casi al final, dentro del `<script>`). Editá **solo eso**:

```js
const CONFIG = {
  brandName : "Gordos' Burgers",
  handle    : "@gordosburgers",
  tagline   : "Las hamburguesas más gordas de Luján de Cuyo",

  whatsapp     : "5492610000000",   // solo números, con código de país
  whatsappText : "¡Hola Gordos! Quiero hacer un pedido 🍔",

  instagram : "gordosburgers",              // sin @
  menuUrl   : "https://tu-carta-online.com",// link real a la carta

  mapsUrl   : "https://www.google.com/maps/...",
  address   : "X3GW+4JP, Luján de Cuyo",

  hours : { /* horarios para el cartel "Abierto ahora" */ }
};
```

- **WhatsApp:** poné el número con código de país y el 9 (Argentina). Ej: `5492613334444`.
- **Horarios:** `0=Dom … 6=Sáb`. `null` = cerrado ese día. Se usa para mostrar *Abierto / Cerrado ahora* en vivo.
- **Logo:** es un ejemplo (ilustración SVG dentro de `.avatar`). Cuando tengas el rebranding, se reemplaza por tu logo (idealmente SVG o PNG con fondo transparente).

## 👀 Probarla localmente

Doble clic en `index.html` — se abre en el navegador. (Para probar el botón *Compartir/Copiar* conviene servirla; ver abajo.)

## 🚀 Publicarla gratis

Cualquiera de estas sirve (arrastrás la carpeta y listo):

- **Netlify Drop** → https://app.netlify.com/drop
- **Vercel** → https://vercel.com (importás la carpeta)
- **GitHub Pages** → subís el repo y activás Pages

Después podés conectar tu dominio (ej. `gs.burger`) desde el panel del hosting.

## 🎨 Cambiar colores

Están todos como variables CSS en `:root` (arriba del `<style>`): `--bg-top`, `--bg-mid`, `--accent`, `--gold`, etc. Cambiás esos valores y se actualiza toda la página.

---
Pendiente: rebranding (logo + colores definitivos) y cargar los enlaces reales.
