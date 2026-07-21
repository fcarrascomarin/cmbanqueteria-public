# CM Banquetería · despliegue público estático

Esta carpeta contiene solo la web pública de CM. No incluye el panel interno.

## Objetivo

Evitar que los clientes vean la pantalla de espera de Render. La web pública debe vivir en un hosting estático como Cloudflare Pages, Netlify, Vercel o GitHub Pages. El backend/panel interno sigue en Render.

## Pasos

1. Desplegar esta carpeta `public-static` como sitio estático.
2. Configurar el dominio público `cmbanqueteria.cl` hacia el hosting estático.
3. Mantener el backend interno en Render.
4. Editar `config.js` y reemplazar:

```js
window.CM_API_BASE = 'https://TU-SERVICIO-INTERNO-RENDER.onrender.com';
```

por la URL real del backend de Render.

5. El botón “Acceso interno” usará automáticamente esa URL y abrirá `/admin.html` en Render.

## Qué queda estático

- Portada pública.
- Restaurant.
- Banquetería.
- Trayectoria.
- Cotización vía WhatsApp.
- Ubicación y footer.

## Qué sigue dependiendo del backend

- Carga del menú del día desde `/api/public/menu/today`.
- Registro de cotizaciones en `/api/public/quotes`.
- Panel interno `/admin.html`.
- Pantalla interna `/pantalla.html`.

Aunque el backend esté dormido, el cliente verá la web pública de inmediato. Solo el menú dinámico o el registro interno pueden tardar; WhatsApp sigue funcionando sin depender del backend.
