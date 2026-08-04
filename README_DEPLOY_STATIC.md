# CM Banquetería · carpeta pública lista para GitHub Pages

Esta carpeta contiene solo la web pública estática.

Backend/panel interno configurado:

```js
window.CM_API_BASE = 'https://cmbanqueteria.onrender.com';
window.CM_ADMIN_URL = 'https://cmbanqueteria.onrender.com/admin.html';
```

Para subir a GitHub Pages, sube el contenido de esta carpeta a la raíz del repositorio público.
No subas la carpeta completa como `public-static/`; sube sus archivos directamente.

El archivo `CNAME` ya contiene:

```txt
cmbanqueteria.cl
```

## Actualización 2026-08-03

- `config.js` apunta a `https://admin.cmbanqueteria.cl` para usar Render solo como backend/panel interno.
- Correo público actualizado a `claudiamendezbanqueteria@gmail.com`.
- La sección ubicación usa la imagen vertical `assets/terraza.jpeg` y un mapa horizontal inferior.
- CM Experience permanece oculto.
